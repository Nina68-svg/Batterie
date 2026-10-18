<h1>Batterie</h1>
<p id="v">lädt …</p>
<script>
fetch('data.json?'+Date.now()).then(r=>r.json()).then(d=>{
  v.textContent = d.percent+' % ('+d.kwh+' kWh), Stand '+d.updated;
});
</script>
