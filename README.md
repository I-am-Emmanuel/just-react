# just-react

import React from 'react'
import { Header, Img } from './TopNavStyle'

const TopNav = ({company_logo, dashboard=false, agent}) => {
  
    return (
        <Header className='top-nav'>
        {dashboard ? (<div><Img src={company_logo} alt="logo" /></div> && <div>{agent.firstName}</div>) 
        : <Img src={company_logo} alt="logo" />
        }
        </Header>
    )
}

export default TopNav
