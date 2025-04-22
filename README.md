# library-starter

Features:

- Bundle with [tsup](https://github.com/egoist/tsup)
- Test with [vitest](https://vitest.dev)

# Usage

### 安装

```bash
pnpm add @oiij/e-charts
```

### 使用

```vue
<script setup lang="ts">
import type { EChartsOption } from '@oiij/e-charts'
import { useECharts } from '@oiij/e-charts'
import { ref } from 'vue'
const option: EChartsOption = ref({
  xAxis: {
    type: 'category',
    data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
  },
})
const { domRef } = useECharts(option)
</script>
<template>
  <div ref="domRef" style="width: 100%; height: 100%;"></div>
</template>
```

## License

MIT
