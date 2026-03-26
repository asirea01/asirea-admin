<template>
  <div class="loader-container">
    <!--     <div class="spinner-border" role="status">
      <span class="visually-hidden">Loading...</span>
    </div> -->
    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24">
      <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
        <path stroke-dasharray="18" d="M12 3c4.97 0 9 4.03 9 9">
          <animate fill="freeze" attributeName="stroke-dashoffset" dur="0.3s" values="18;0" />
          <animateTransform attributeName="transform" dur="1.5s" repeatCount="indefinite" type="rotate"
            values="0 12 12;360 12 12" />
        </path>
        <path stroke-dasharray="60"
          d="M12 3c4.97 0 9 4.03 9 9c0 4.97 -4.03 9 -9 9c-4.97 0 -9 -4.03 -9 -9c0 -4.97 4.03 -9 9 -9Z" opacity="0.3">
          <animate fill="freeze" attributeName="stroke-dashoffset" dur="1.2s" values="60;0" />
        </path>
      </g>
    </svg>
  </div>
</template>
<style scoped lang="scss">
.loader-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;

  .spinner-border {
    color: var(--accent-color);
    width: 4rem;
    height: 4rem;
    border-width: 6px;
  }
}
</style>
