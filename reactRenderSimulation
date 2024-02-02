function render(reactElement, containerDOMElement) {
  const tag = reactElement.type
  const element = document.createElement(tag);

  // properties 
  const properties = reactElement.props;
  element.innerText = reactElement.children;
  for (prop in properties){
    element.setAttribute(`${prop}`, `${properties[prop]}`)
  }

  // render
  containerDOMElement.appendChild(element)  
}

const reactElement = {
  type: 'a',
  props: {
    href: 'https://wikipedia.org/',
  },
  children: 'Read more on Wikipedia',
};

const containerDOMElement =
  document.querySelector('#root');

render(reactElement, containerDOMElement);
