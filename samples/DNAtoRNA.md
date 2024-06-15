# DNA to RNA
<label for="dna">DNA to convert to RNA</label><input type="text" id="dna" size="10"><button id="toRNA">to RNA</button>
<p>Result: <span id="rna"></span></p>
<script>
const dnaToRna = {G: "C",C:"G",T:"A",A:"U"};
const toRna = (dna) => dna.split("").map(d => dnaToRna[d]).join("");
  document.getElementById("toRNA").addEventListener("click", () => {
    let DNA = document.getElementById("dna").value;
    DNA = DNA.toUpperCase();
    document.getElementById("rna").innerText = toRna(DNA);
  });
</script>