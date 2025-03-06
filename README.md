import React from 'react';
import { Header, Img, NameContainer } from './TopNavStyle';

const TopNav = ({ company_logo, dashboard = false, agent }) => {
  return (
    <Header className='top-nav'>
      {dashboard ? (
        <>
          <Img src={company_logo} alt="logo" />
          <NameContainer>{agent.firstName}</NameContainer>
        </>
      ) : (
        <Img src={company_logo} alt="logo" />
      )}
    </Header>
  );
};

export default TopNav;
✅ TopNavStyle.js (Fixed Styles)
jsx
Copy
Edit
import styled from 'styled-components';

export const Header = styled.header`
  display: flex;
  align-items: center;
  padding: 0 20px;
  background-color: green;
  color: white;
  height: 50px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
`;

export const Img = styled.img`
  width: 50px;
  height: 40px;
  margin-right: 10px; /* Add space between image and text */
`;

export const NameContainer = styled.div`
  font-size: 16px;
  font-weight: bold;
`;
✅ App.js (No Changes, Just Ensuring Proper Usage)
jsx
Copy
Edit
import React from 'react';
import TopNav from './Utils/components/TopNav/TopNav';
import random_logo from './images/random_logo.png';

function App() {
  return (
    <>
      <TopNav company_logo={random_logo} dashboard={true} agent={{ firstName: 'Alice' }} />
    </>
  );
}

export default App;
