.doc .collection is how you query firestore db and get back an object
.doc used for crud and gets document snapShot object
.collection get query snapShot obejct
.get pulls out snapShot object to detrmine with our code wether or not there is a reference

query refObject and query snapShot is what you get from fire store

ref object that represents current place in database
  get by calling firestore.doc('/users/:userId')
  or firestore.collections('/users')
  does not have actual data of the collections, but properties that tell us details(id or path etc) about it
  or the Snapshot object which gives us the data we are looking for

to retreive the snapShot call .get()


queryReference represents current place in database
  get by calling firestor.doc(path) or firestore.collection(path)
  does not have actual data but properties that tell us about it
      docRef is used for crud
        .set() to create
        .get() to get the data
        .update() to update
        .delete() to delete
      we can add documents to collections as long as we use .add() method collectionRef.add({value: prop})


to get data we have to get the snapShot object by using the ref object by calling.getmethod on docref or collection ref.

docref returns documentsnapshot object
collection ref returns a querysnapshot object

docsnapshot allows to chec if document exists using .exists property
we can get actual properties by calling .data() which returns a json object of the data

querySnapShot object from collection ref object
