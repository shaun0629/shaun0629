var textureLoader = new THREE.TextureLoader();
var texture = textureLoader.load("cit.png"); var mat = new THREE.MeshPhongMaterial(); 
mat.map = texture;
// 箱を作成
var geometry = new THREE.BoxGeometry(1, 1, 1);
//var material = new THREE.MeshPhongMaterial({ color: 0xffffff }); //var box = new THREE.Mesh(geometry, material);
var box = new THREE.Mesh(geometry, mat); box.position.z = -5;
scene.add(box);
