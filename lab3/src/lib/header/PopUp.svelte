<script>
  import { popUpMessage } from '../../store';
  $: popUpMessage && setTimeout(() => ($popUpMessage = ''), 2000);
</script>

<p>
  {$popUpMessage}
</p>

<style>
  p {
    background-color: red;
    border-radius: 15px;
    position: fixed;
    right: 30px;
    bottom: 30px;
    padding: 10px 15px;
    z-index: 6;
  }
</style>
