<script> 
 // gjjj
let tanggal = '';
 
 function runDay() {
  const time = new Date()
  tanggal = time.getUTCDay() +','+ time.getDate() +'-'+ time.getMonth() +'-'+ time.getFullYear()
  setTimeout ( runDay , 24 * 60 * 60 * 1000 )
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
