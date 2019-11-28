Well of Ideas - Easy Version

function DNAStrand(dna){
  let r = '';
  for(let i = 0; i < dna.length; i++){
      if(dna[i] === 'A') r +='T';
      if(dna[i] === 'T') r += 'A';
      if(dna[i] === 'C') r += 'G';
      if(dna[i] === 'G') r += 'C';
    }
    return r;
}