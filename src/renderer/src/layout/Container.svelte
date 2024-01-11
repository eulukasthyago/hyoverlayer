<script lang="ts">
  import '../css/global.css'
</script>

<div>
  <div class="draggable flex justify-between p-2 bg-gray-900 text-gray-50">
    <div>Nome do aplicativo</div>
    <div class="no-draggable flex gap-2">
      <button type="button">M</button>
      <button type="button">m</button>
      <button type="button">X</button>
    </div>
  </div>
  <div class="bg-gray-50 w-full h-7 flex-row flex-wrap items-center px-2 hidden">
    <ul>
      <li>
        <a href="#menu">Menu</a>
        <ul>
          <li>
            <a href="#submenu">Submenu</a>
          </li>
        </ul>
      </li>
    </ul>
  </div>
  <slot />
</div>
