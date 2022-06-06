<script> 
 // gjjj
let tanggal = '';
 
 function runDay() {

const Xmas95 = new Date();
const weekday = Xmas95.getDay();

 const options = { weekday: 'long'};
console.log(new Intl.DateTimeFormat('en-US', options).format(Xmas95));
const today = new Date();
  tanggal =
+','+ today.getDate() +'-'+ today.getMonth() +'-'+ today.getFullYear()

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


<h4> {tanggal} </h4>
<h4>Jam: {jam}</h4>
<p>
 <table>
  <tr>
   <td>Beranda</td>
   <td>Akun</td>
  </tr>
</table>
