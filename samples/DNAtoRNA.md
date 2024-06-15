# DNA to RNA
<label for="dna">DNA to convert to RNA</label><input type="text" id="dna" size="10"><button id="toRNA">to RNA</button>
<p id="rna"></p>
<script>
const dnaToRna = {G: "C",C:"G",T:"A",A:"U"};
const toRna = (dna) => dna.split("").map(d => dnaToRna[d]).join("");
  document.getElementById("toRNA").addEventListener("click", () => {
    let DNA = document.getElementById("dna").value;
    document.getElementById("rna").value = toRna(DNA);
  });
</script>