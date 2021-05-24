# quote-React
node 
C:\Users\guido2020>node -v
v16.0.0

C:\Users\guido2020>npm -v


react
github.com/facebook/create-react-app
github.com/facebook/create-react-app


cmd
npx create-react-app prestamos

descargarmos de chorme web store react developer tools

cmd
cd prestamos/

cmd
npm start


cmd
npm run build <--- para crear un build de produccion una carpeta de react para subir a git 


https://gist.github.com/juanpablogdl/194c15d376391a67c46dd08817bf9ae4
https://tobiasahlin.com/spinkit/
///////////////////////////////////////////////////////////////////////
luego la carpeta prestamos abrimos en VISUAL STUDIO

instalamos en visual studio react 
ES7 React/Redux/GraphQL/React-Native snippets
Simple React Snippets


luego abrimos esta pagina para scar el css
https://cdnjs.com/
buscamos skeleton 
y copiamos el skeleton link tag
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/normalize/8.0.1/normalize.min.css" integrity="sha512-NhSC1YmyruXifcj/KFRWoC561YpHpc5Jtzgvbuzx5VozKpWvQ+4nXhPdFgmx8xqexRcpAglTj9sIBWINXa8x5w==" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css" integrity="sha512-EZLkOqwILORob+p0BXZc+Vm3RgJBOe1Iq/0fiI7r/wJgzOFZMlsqTa29UEl6v6U6gsV4uIpsNZoV32YZqrCRCQ==" crossorigin="anonymous" />
  
luego creamos la carpeta Componentes creamos Header.js

escribimos 
import React from 'react';

function Header(){
    return(
        <div className="App">
            <h1> Hellos react </h1>

        </div>
    );
}

export default Header;

import react  from 'react';  
import Header from './componentes/Header';

function App() {
  return (
    <div className="App">
          <Header/>
          <Header/>
          <Header/>
          <Header/>
          <Header/>
          
    </div>
  );
}

export default App;





REACT JS
/////////////////////////////////////////////////////////////////////////////////////////////////////////
FRAGMENT 
es como div para no generar contenido html extra 

los PROPS
los pro estan dentro del Header como titulos , descripcion TAMBIEN llevan Fragment
y para llamarlo usar {} dentro d esto usamos JS

CONST HEADER 
Hacemos mas corto el codigo y aparte podemos meter JS cuando quieramos mas implisito

IMR = importar REACT
sfc = crear estructura CONST



////////////////////////////////////////////////////////////////////////////////////////////////////////
FRAGMENT 
es como div para no generar contenido html extra 

import react ,{Fragment} from 'react';
import Header from './componentes/Header';

function App() {
  return (
    <Fragment>
          <Header/>
          <Header/>
          <Header/>
          <Header/>
          <Header/>
          
    </Fragment>
  );
}

export default App;

///////////////////////////////////////////////////////////////
los PROPS
los pro estan dentro del Header como titulos , descripcion 


app.js
import react ,{Fragment} from 'react';
import Header from './componentes/Header';

function App() {
  return (
    <Fragment>
          <Header
           titulo="Cotizador de numeros "  // esto serian los PROPS
           descripcion = " utuliza el formulario y obten una cotizacion "
          />
        
          
    </Fragment>
  );
}

export default App;


/////carpeta componente crear con Mayuscula js
Header.js 

import React, { Fragment } from 'react';

function Header(titulo){

    //console.log(props);// como leer un props

    return(
            <Fragment>
            <h1>{titulo.titulo} </h1> 
            <p>{titulo.descripcion}</p>
            <p>{2+2}</p>
            </Fragment>
    );  // sino ponemos los corchetes lo interpreta como html con corchete como JS
}

export default Header;

/////////////////////////////////////////////////////////////////////////////////

CONST HEADER 
Hacemos mas corto el codigo y aparte podemos meter JS cuando quieramos mas implisito


import React from 'react'

const Header = ({titulo}) => (  // esta forma tenemos un codigo mas limnpio y mas corto
     
        <h1>{titulo} </h1> 
      );
export default Header;




