<template>
  <div class="mb-4 space-y-2" v-for="color in colors">
    <div class="text-base">{{ color }}</div>
    <div class="flex space-x-1">
      <div
        v-for="shade in [
          '50',
          '100',
          '200',
          '300',
          '400',
          '500',
          '600',
          '700',
          '800',
          '900',
        ]"
        class="h-8 w-8 rounded-md"
        :class="colorShades[color][shade]"
      ></div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Color',
  computed: {
    colors() {
      return [
        'gray',
        'blue',
        'green',
        'red',
        'orange',
        'yellow',
        'teal',
        'violet',
        'cyan',
        'amber',
        'pink',
        'purple',
      ]
    },
    colorShades() {
      return {
        gray: {
          50: 'bg-gray-50',
          100: 'bg-gray-100',
          200: 'bg-gray-200',
          300: 'bg-gray-300',
          400: 'bg-gray-400',
          500: 'bg-gray-500',
          600: 'bg-gray-600',
          700: 'bg-gray-700',
          800: 'bg-gray-800',
          900: 'bg-gray-900',
        },
        blue: {
          50: 'bg-blue-50',
          100: 'bg-blue-100',
          200: 'bg-blue-200',
          300: 'bg-blue-300',
          400: 'bg-blue-400',
          500: 'bg-blue-500',
          600: 'bg-blue-600',
          700: 'bg-blue-700',
          800: 'bg-blue-800',
          900: 'bg-blue-900',
        },
        green: {
          50: 'bg-green-50',
          100: 'bg-green-100',
          200: 'bg-green-200',
          300: 'bg-green-300',
          400: 'bg-green-400',
          500: 'bg-green-500',
          600: 'bg-green-600',
          700: 'bg-green-700',
          800: 'bg-green-800',
          900: 'bg-green-900',
        },
        red: {
          50: 'bg-red-50',
          100: 'bg-red-100',
          200: 'bg-red-200',
          300: 'bg-red-300',
          400: 'bg-red-400',
          500: 'bg-red-500',
          600: 'bg-red-600',
          700: 'bg-red-700',
          800: 'bg-red-800',
          900: 'bg-red-900',
        },
        orange: {
          50: 'bg-orange-50',
          100: 'bg-orange-100',
          200: 'bg-orange-200',
          300: 'bg-orange-300',
          400: 'bg-orange-400',
          500: 'bg-orange-500',
          600: 'bg-orange-600',
          700: 'bg-orange-700',
          800: 'bg-orange-800',
          900: 'bg-orange-900',
        },
        yellow: {
          50: 'bg-yellow-50',
          100: 'bg-yellow-100',
          200: 'bg-yellow-200',
          300: 'bg-yellow-300',
          400: 'bg-yellow-400',
          500: 'bg-yellow-500',
          600: 'bg-yellow-600',
          700: 'bg-yellow-700',
          800: 'bg-yellow-800',
          900: 'bg-yellow-900',
        },
        teal: {
          50: 'bg-teal-50',
          100: 'bg-teal-100',
          200: 'bg-teal-200',
          300: 'bg-teal-300',
          400: 'bg-teal-400',
          500: 'bg-teal-500',
          600: 'bg-teal-600',
          700: 'bg-teal-700',
          800: 'bg-teal-800',
          900: 'bg-teal-900',
        },
        violet: {
          50: 'bg-violet-50',
          100: 'bg-violet-100',
          200: 'bg-violet-200',
          300: 'bg-violet-300',
          400: 'bg-violet-400',
          500: 'bg-violet-500',
          600: 'bg-violet-600',
          700: 'bg-violet-700',
          800: 'bg-violet-800',
          900: 'bg-violet-900',
        },
        cyan: {
          50: 'bg-cyan-50',
          100: 'bg-cyan-100',
          200: 'bg-cyan-200',
          300: 'bg-cyan-300',
          400: 'bg-cyan-400',
          500: 'bg-cyan-500',
          600: 'bg-cyan-600',
          700: 'bg-cyan-700',
          800: 'bg-cyan-800',
          900: 'bg-cyan-900',
        },
        amber: {
          50: 'bg-amber-50',
          100: 'bg-amber-100',
          200: 'bg-amber-200',
          300: 'bg-amber-300',
          400: 'bg-amber-400',
          500: 'bg-amber-500',
          600: 'bg-amber-600',
          700: 'bg-amber-700',
          800: 'bg-amber-800',
          900: 'bg-amber-900',
        },
        pink: {
          50: 'bg-pink-50',
          100: 'bg-pink-100',
          200: 'bg-pink-200',
          300: 'bg-pink-300',
          400: 'bg-pink-400',
          500: 'bg-pink-500',
          600: 'bg-pink-600',
          700: 'bg-pink-700',
          800: 'bg-pink-800',
          900: 'bg-pink-900',
        },
        purple: {
          50: 'bg-purple-50',
          100: 'bg-purple-100',
          200: 'bg-purple-200',
          300: 'bg-purple-300',
          400: 'bg-purple-400',
          500: 'bg-purple-500',
          600: 'bg-purple-600',
          700: 'bg-purple-700',
          800: 'bg-purple-800',
          900: 'bg-purple-900',
        },
      }
    },
  },
}
</script>
