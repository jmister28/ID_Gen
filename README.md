# ID_Gen
ID_Gen is a database service using the Firebase™ API. You can make your own live news broadcasts, a texting program, and so much more.
# Installation
We make it easy to install our program into any HTML document just put this `<script src='https://cdn.firebase.com/js/client/2.0.4/firebase.js'></script>` and `    <script src='https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js'></script>`
 in your `<head>` tag 
# Use
To use our program follow our example below
`<html>`
`<head>`
`<script src='https://cdn.firebase.com/js/client/2.0.4/firebase.js'></script>`
`<script src='https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js'></script>`
`</head>`
  `<body>`
    `<script>`
     `var id_gen = new Firebase ('id-gen.firebaseIO.com')`
     `id_gen.push({object_here: data_here, different_object_here: data_here});`
     `id_gen.on("child_added", function(snapshot) {`
       `console.log("your_id: " + snapshot.name());`
       `console.log("data: " + snapshot.val());`
      `});`
     `</script>`
  `</body>`
 `</html>`
