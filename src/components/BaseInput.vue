<template>
  <label v-if="label">{{ label }}</label>
  <input
    :placeholder="label"
    v-bind="$attrs"
    :value="modelValue"
    @input="$emit('update:modelValue', $event.target.value)"
    class="field"
  />

  <p
    v-if="error"
    class="errorMessage"
  >
{{ error }}
  </p>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: ''
    },
    modelValue: {
      type: [String, Number],
      default: ''
    },
    error: {
      type: String,
      default: ''
    }
  }
}
</script>
