<script setup lang="ts">
import { ref, computed } from 'vue';
import { Note, Interval, Scale, ScaleType, Chord } from 'tonal';

const scaleNames = Scale.names();
const note = 'c5';
const scale = scaleNames?.[8];
const scaleName = `${note} ${scale}`;
const fullScale = Scale.get(scaleName);
</script>

<template>
  <div>
    <pre>Test</pre>
    <pre>Scale name: {{ scale }}</pre>
    <pre>Scale notes: {{ fullScale?.notes }}</pre>
  </div>
</template>
