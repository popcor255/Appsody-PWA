<script>
  import { count } from "../store/store.js";

  /**
   * Increases the count variable from the store by 1
   */
  function incrementCount() {
    count.set($count + 1);
  }
</script>

<style type="text/sass">
  .button {
    background-color: #4CAF50; /* Green */
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
  }
</style>

<div class="flex items-center justify-center h-screen bg-gray-200">
  <button class="button" on:click={() => incrementCount()}>
    Count is {$count}
  </button>
</div>
