<template>
  <h3 :class="$style['m-class']">using Module CSS with $ Syntax (Kabab-case)</h3>
</template>

<style module>
/* Kabab-case */
.m-class {
  background-color: firebrick;
  color: white;
}
</style>
