    ------------------------------------------------------------------    
                know about js Dom 02  <Start>
    -------------------------------------------------------------------


    // //innerHtml and innerText er modde difference ki ?? 

    // const h1 = document.querySelector(".h1")
    // console.log(h1.innerHTML); /// innerhtml pura html ta ke show korai :
    // // output : Hello This is <span>Nishat</span>
    
    // console.log(h1.innerText); // Hello This is Nishat ; sudu text ta ke show korai 

    // // kono ekta div er maje kemne arrekta tag ba div niben ?
    // const div = document.createElement("div")
    // const p = document.createElement("p")
    // p.innerHTML = "this is "
    // div.appendChild(p) // div er bitore p tag ke nilam 
    // console.log(div);
    // // output : <div><p></p></div>

    // append and appendChild er maje difference ki ??? 
    // append tag string sob kicu nei 
    // append child sudu matro tag nei ,
    // Example
    //=================================================
    const div2 =document.createElement("div")
    const p = document.createElement("p")
    p.innerHTML = "Hello nishat"
    div2.append(p)
    console.log(div2);
    // ekane append tag o nei and text o nei jemon text er Example
    //--------------------------------------------------
    const div3 =document.createElement("div")
    div3.append("xyz")
    console.log(div3);
    //--------------------------------------------------
    // deken div er bitore sudu text ke o se nicce 
    // kintu 
    //=================================================
    const div4 =document.createElement("div")
    const p3 = document.createElement("p")
    p3.innerHTML = "Hello nishat p3"
    div4.appendChild(p3) // se tag ke thik e nicce 
    console.log(div4);
    // <div><p>Hello nishat p3</p></div> // 
    //--------------------------------------------------
    // const div5 =document.createElement("div")
    // div5.appendChild("Hello Nishat div5") // se tag ke thik e nicce 
    // console.log(div5); // ekon kintu output se error dekacce karon appenchild text nei na 
    //--------------------------------------------------
    //=================================================

    // nextElementsibling/nextsibling eta ki ?? 
    // next sibling 
    // aetar mane holo ek vai brother , 
    // jemon doren body er vitore ul tag and script tag ase tar mane holo
    // ul er sibling holo script tag
    // tobe jodi script tag er space thake taile kintu nextsibling se text ke nibe

    const ul = document.querySelector(".ul")
    console.log(ul.nextSibling); //text ; karon ul er pore gap ase
    console.log(ul.nextSibling); // <script src="script.js"></script> ; karon gap del korsi 

    // ar nextElement sibling er mane holo 
    // dore nen ul and script tag ase and maje gap o ase 
    // taile ul er nextElementSibling holo script tag 
    // karon ekane bolsi nextElemnet sibling

    // so ekon doren ul er li  gulo te por por kemne jabo samner dike

    const ul1 = document.querySelector(".ul1")
    const Allchild = ul1.children
    console.log(Allchild[0].nextElementSibling.innerHTML); // <a href="#">two</a>


    // so ekon doren ul er li  gulo te pecone theke kemne jabo 
    const ul2 = document.querySelector(".ul2")
    console.log(ul2.children[4].previousElementSibling.innerHTML); 
    // <a href="#">four</a>
    console.log(ul2.parentNode); // ul er parent holo body


    // ekon doren ami children korte cie na taile kemne hobe

    const ul3 = document.querySelector(".ul3 li") //ul er bitor je li ase
    console.log(ul3);// sudu ekta li paice , sobgulo pete use querselectAll

    const ul4 = document.querySelectorAll(".ul4 li") //ul er bitor je sobgulo (queryselectorALl) li ase
    console.log(ul4);// NodeList(5) [li, li, li, li, li]

    ------------------------------------------------------------------    
                know about js Dom 02  <End>
    -------------------------------------------------------------------