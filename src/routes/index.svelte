<script> 
 // gjjj
let tanggal = '';
 
 function runDay() {
  const time = new Date()
  tanggal = time.getDay() +','+ time.getDate() +'-'+ time.getMonth() +'-'+ time.getYear()
  serTimeout(runDay, 24*60*60*1000)
}
 
 runDay()
 
let jam = '';
 
function runTimer() {
  const date = new Date()
  jam = date.getHours() +':'+ date.getMinutes() +':'+ date.getSeconds()
  setTimeout(runTimer, 1000)
} 
 
runTimer()
</script>
<h1> {tanggal} </h1>
<h1>Jam: {jam}</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
