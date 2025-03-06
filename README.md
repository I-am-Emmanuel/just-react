import React from 'react'
import { Header, Img } from './TopNavStyle'

const TopNav = ({company_logo, dashboard=false, agent}) => {
  
    return (
        <Header className='top-nav'>
        {dashboard ? (
        
        <div>
        <Img src={company_logo} alt="logo" />
        </div> &&
         <div>{agent.firstName}</div>
        
        ) : (
        <Img src={company_logo} alt="logo" />
        )}
        </Header>
    );
};

export default TopNav

import styled from 'styled-components';



 export const Header = styled.header`
  display: flex;
  align-items: center;
  padding: 0 80px;
  background-color: green;
  color: white;
  height: 50px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
`;

export const Img = styled.img`
  width: 50px;
  height: 40px;
  ${'' /* border-radius: 50%; */}
`;

export const Div = styled.div`
  display: flex;
  align-items: center;
  display: grid;
  padding-left: 20px;
`;

// import logo from './logo.svg';
import TopNav from './Utils/components/TopNav/TopNav';
import React  from 'react';
import random_logo from './images/random_logo.png';

function App() {
  // const handleNameChange = () => {
  //   const names = ['Alice', 'Emily', 'Kate'];
  //   const int = Math.floor(Math.random() * 3);
  //   return names[int];
  // }
  
  return (
    <>
      <TopNav company_logo={random_logo}
              dashboard={true} 
              agent={{firstName: 'Alice'}} />   
      
    </>
  );
}

export default App;
