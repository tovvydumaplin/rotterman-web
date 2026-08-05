<script setup>
/**
 * BaseButton - Reusable button component
 * 
 * Props:
 * - variant: 'primary' | 'secondary' | 'danger' (default: 'primary')
 * - size: 'sm' | 'md' | 'lg' (default: 'md')
 * - disabled: boolean
 * - loading: boolean
 * - type: 'button' | 'submit' | 'reset' (default: 'button')
 */

defineProps({
  variant: {
    type: String,
    default: 'primary',
    validator: (value) => ['primary', 'secondary', 'danger', 'link'].includes(value)
  },
  size: {
    type: String,
    default: 'md',
    validator: (value) => ['xs', 'sm', 'md', 'lg'].includes(value)
  },
  disabled: {
    type: Boolean,
    default: false
  },
  loading: {
    type: Boolean,
    default: false
  },
  type: {
    type: String,
    default: 'button'
  }
})
</script>

<template>
  <button
    :type="type"
    :disabled="disabled || loading"
    :class="[
      'base-button',
      `base-button--${variant}`,
      `base-button--${size}`,
      { 'base-button--loading': loading }
    ]"
  >
    <span v-if="loading" class="base-button__spinner"></span>
    <slot />
  </button>
</template>

<style scoped>
  .base-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
    font-weight: 600;
    border: 1px solid transparent;
    border-radius: 5px;
    cursor: pointer;
    transition: all 0.2s ease;
  }

  .base-button:disabled {
    opacity: 0.6;
    cursor: not-allowed;
  }

  /* Variants */
  .base-button--primary {
    background-color: #186534;
    color: white;
  }
  .base-button--primary:hover:not(:disabled) {
    background-color: #14522b;
  }

  .base-button--secondary {
    background-color: transparent;
    color: #186534;
    border: 1px solid #186534;
  }
  .base-button--secondary:hover:not(:disabled) {
    border-color: rgba(139, 173, 0, 0.4);
    color: #8BAD00;
    background-color: transparent;
  }

  .base-button--danger {
    background-color: #ef4444;
    color: white;
  }
  .base-button--danger:hover:not(:disabled) {
    background-color: #dc2626;
  }

  .base-button--link {
    background-color: transparent;
    color: #3B3B3B;
    padding: 0;
  }
  .base-button--link:hover:not(:disabled) {
    color: rgb(27, 27, 27);
  }

  /* Sizes */
  .base-button--xs {
    padding: 0.25rem 0.625rem;
    font-size: 0.75rem;
  }

  .base-button--sm {
    padding: 0.5rem 1rem;
    font-size: 0.875rem;
  }
  .base-button--md {
    padding: 1rem 2rem;
    font-size: 1rem;
  }
  .base-button--lg {
    padding: 1rem 2rem;
    font-size: 1.125rem;
  }

  /* Loading spinner */
  .base-button__spinner {
    width: 1rem;
    height: 1rem;
    border: 2px solid currentColor;
    border-right-color: transparent;
    border-radius: 50%;
    animation: spin 0.75s linear infinite;
  }

  @keyframes spin {
    to { transform: rotate(360deg); }
  }
</style>