what is react:
react is a library of javascript to ctreate frontend ui components.(it help to create single page webapplications)
HOW TO SETUP REACT:
use create react app to create react app and then use bpm install commands to initialize node modules. OR you can use vite to create react project and the initializa the node modules using npm install
WHAT ARE COMPONENTS:
component are functions thet are reusable
PROPS:
props are the properties that are use to pass data between components
HOOKS:
hooks are functions that are use to accesss features of react
SOME POPULAR HOOKS:
(I) USE STATE:it is use to change the state it take a intial value and a function on which the value of state is changed i.e. usestate[count(state),setcount(method)]=usestate(initialvalue you can give any initial value could be 0)
(II)use callback: use call back is used to keep the function in cache who's value you might need in othe components or functions. you pass function and its dependcies i.e. usecallback(function,[dependecies in array])
(III) USE REF" use ref is used when you want to take a reference of a variable useref(defaultvalue)
(iv)USE EFEECT: use effect is used to add effecs when a component is mounted or unmounted.
REACT ROUTER DOM:
react router is installed using the command npm install react-router-dom
react router is used to switch pages without reloading it uses link tag in place of <a> tag to switch pages with out reload it has to attribute in place of href
to use react route we first have to create react router using createbrowserouter in which we have to give object that contain the path and elements you can also give nested paths
i,e. const router=createbrowserrouter([{
path:'/'
element:(can be any component),
children[{
path:''
element:(any component)
}]
}])
now you have to pass the routing variable that you created to rout provider as a prop
i.e. <routerprovider router=router>
