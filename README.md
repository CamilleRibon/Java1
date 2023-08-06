
for ( var i=1; i<=5; i++){
console.log(i);
}

let numberOfNFTs = 0;

function mintNFT(name, description, school){
const nft = {
name: name,
description: description,
school: school,
};

numberOfNFTs++;
return nft;
}

const nfts = [];

function listNFTs() {
for (const nft of nfts){
console.log("Name: " +nft.name);
console.log("Description: " +nft.description);
console.log("School: " +nft.school);
console.log("---");
}
}
function  getTotalSupply(){
console.log("Total Supply: " + numberOfNFTs);
}

const nft1 = mintNFT("Camille Ribon", "Cumlaude", "La Salle");
const nft2 = mintNFT("Archie Calma", "Magna Cumlaude", "FEU");
const nft3 = mintNFT("Denyce Ann Calma", "Summa Cum Laude", "NTC");

nfts.push(nft1, nft2, nft3);

listNFTs();

getTotalSupply();
