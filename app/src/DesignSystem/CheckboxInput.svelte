<script>
  export let checked = null;
</script>

<style>
  .wrapper {
    display: inline-flex;
    position: relative;
    user-select: none;
    cursor: pointer;
  }

  input {
    height: 24px;
    width: 24px;
    -webkit-appearance: none;
    appearance: none;
    outline: none;
    cursor: pointer;
    background: url('data:image/svg+xml;utf8,<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><circle cx="12" cy="12" r="11" stroke="%2390A0AF" stroke-width="2"/></svg>')
      no-repeat;
  }

  input:checked {
    background: url('data:image/svg+xml;utf8,<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><circle cx="12" cy="12" r="12" fill="%23E074CB"/><path fill-rule="evenodd" clip-rule="evenodd" d="M18.7071 8.29289C19.0976 8.68342 19.0976 9.31658 18.7071 9.70711L11.7071 16.7071C11.3166 17.0976 10.6834 17.0976 10.2929 16.7071L6.29289 12.7071C5.90237 12.3166 5.90237 11.6834 6.29289 11.2929C6.68342 10.9024 7.31658 10.9024 7.70711 11.2929L11 14.5858L17.2929 8.29289C17.6834 7.90237 18.3166 7.90237 18.7071 8.29289Z" fill="%23FFFFFF"/></svg>')
      no-repeat;
  }

  span {
    margin-left: 14px;
  }
</style>

<label class="wrapper">
  <input type="checkbox" bind:checked />
  <span>
    <slot />
  </span>
</label>
