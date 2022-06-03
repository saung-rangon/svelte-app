<script> 
 // gjjj

let jam = '';
 
const runTimer() {
  const date = new Date()
  jam = date.getHour() +':'+ date.getMinutes() +':'+ date.getSeconds()
  setTimeout(runTimer, 1000)
} 
 
runTimer()
</script>

<h1>Jam: {jam}</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
