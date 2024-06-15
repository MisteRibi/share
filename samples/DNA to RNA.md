# DNA to RNA
<label for="dna">DNA to convert to RNA</label><input type="text" id="dna"><button id="toRNA">to RNA</button>
<p id="rna"></p>
<script>document.getElementById("toRNA").addEventListener("click", () => {
    let DNA = document.getElementById("dna").value;
    document.getElementById("rna").value = DNA + "lol";
  });
</script>