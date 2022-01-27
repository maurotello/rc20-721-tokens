# Unidad4_EIP_ERC20_ERC721

## El orden en que vamos a ver estos contratos en la siguiente:

### 1 - EITToken.sol
Token ERC20 de ejemplo que vamos a hacer el "deploy" en una red local

### 2 - BasicImplERC20.sol
Es un ejemplo de implementación básica de la intereface IERC20 si no usaramos la implementación de OpenZeppelin
Está todo comentado para evitar que que sea compilado y de errores.

### 3 - NFTEjemplo.sol
Implementación de un token no fungible (NFT) utilizando las implementaciones del estandar ERC-721 de OpenZeppelin
Tambiénn haremos el deploy local con truffle develop

### 4 - NFTImplERC721.sol
Ejemplos de las distintas funcionalidades y particularidades en el caso de implementar el estadar ERC-721.
También está todo comentado para evitar que que sea compilado y de errores.

### 5 - UPLOAD FILES TO IPFS FROM BROWSER
- https://anarkrypto.github.io/upload-files-to-ipfs-from-browser-panel/public/
- https://nft.storage/
- https://jsonkeeper.com/

- Implementar ERC-721 
	Vemos ejemplo GameItem
	Vemos implementacion de interface
	_setTokenURI: https://nft.storage/

	 
	Compilamos
	```
	Truffle Develop
	const game = await GameItem.deployed();

	game.awardItem("0x52b0f942ccaa9f6bc9fe41ae2002f602d2a99a9d", "https://bafybeihiufoeircpkiav3cjqzhpx44d5epjotfabpftydx5hqhkvhm2zma.ipfs.infura-ipfs.io/") 
	
  game.ownerOf(1)
	game.tokenURI(1)
	```

Address contrato (será distinto en cada deploy)
0x3e23e783ab2a0b5258AefCB28853A46a9527d6E7

ipfs uri
https://bafybeihiufoeircpkiav3cjqzhpx44d5epjotfabpftydx5hqhkvhm2zma.ipfs.infura-ipfs.io/

contenido
{
  "name": "Martillo de Thor",
  "description": "Mjölnir, el legendario martillo del dios nórdico del trueno.",
  "image": "https://game.example/item-id-8u5h2m.png",
  "strength": 20
}