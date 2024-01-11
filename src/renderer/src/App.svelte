<script lang="ts">
  import Container from './layout/Container.svelte'

  const ipc = window.electron.ipcRenderer

  const handleOpenOverlay = (): void => {
    ipc.invoke('overlay', true)
  }
  const handleCloseOverlay = (): void => {
    ipc.invoke('overlay', false)
  }
</script>

<Container>
  <div class="p-2">
    <div class="pt-4">
      <button on:click={handleOpenOverlay}>Open Overlayers</button>
      <br />
      <button on:click={handleCloseOverlay}>Close Overlayers</button>
    </div>
  </div>
</Container>
