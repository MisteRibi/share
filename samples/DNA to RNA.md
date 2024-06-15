# DNA to RNA
<input type="text" id="dna"><button id="toRNA">
<p id="rna">lol</p>
<script>document.getElementById("toRNA").addEventListener("click", () => {
    let DNA = document.getElementById("dna").value;
    
    document.getElementById("rna").value = DNA + "lol";
  });
</script>