# github
//it is for board infinity 
import React, { useState } from 'react';

const App = () => {
  
  const [name ,setName] = useState("");
  const [fullName,setFullName] = useState();

  const InputEvent = (event) =>{
    console.log(event.target.value);
    setName(event.target.value);
    };
    const onSubmit = () =>{
      
      setFullName(" abhishek profile id 21182294=> followers 600k and following=>99k");
    }
return(
<>
   <div>
    <h1>
                    GithubCompare
    </h1>
    
    <input type="text" placeholder="username" 
    onChange={InputEvent} 
    value={name}
    />
    <button onClick={onSubmit} >
      Compare
    </button>
    
    {fullName}
   </div>
   </>
);
};

export default App;
