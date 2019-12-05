<!-- 1 -->
const JSX = <h1>Hello JSX!</h1>;
<!-- 2 -->
const JSX = <div>
    <h1>h1 tag</h1>
    <p>p tag </p>
    <ul>
        <li> li 1</li>
        <li> li 2</li>
        <li> li 3</li>
    </ul>
</div>
<!-- 3 -->
const JSX = (
  <div>
  {/* main div*/}
    <h1>This is a block of JSX</h1>
    <p>Here's a subtitle</p>
  </div>
);

<!-- 4 -->

const JSX = (
  <div>
    <h1>Hello World</h1>
    <p>Lets render this to the DOM</p>
  </div>
);
// change code below this line
ReactDOM.render(JSX,document.getElementById('challenge-node'))

<!-- 5 -->
const JSX = (
  <div className="myDiv">
    <h1>Add a class to this div</h1>
  </div>
);
<!-- 6 -->

const JSX = (
  <div>
    <h2>Welcome to React!</h2> <br />
    <p>Be sure to close all tags!</p>
    <hr />
  </div>
);

<!-- 7 -->

const MyComponent = function() {
  // change code below this line
return(
  <div>MyComponent</div>
);
  // change code above this line
}

<!-- 8 -->

class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    // change code below this line

    return (
      <div>
      <h1>Hello React!</h1>
      </div>
    )


    // change code above this line
  }
};


<!-- 9 -->
const ChildComponent = () => {
  return (
    <div>
      <p>I am the child</p>
    </div>
  );
};

class ParentComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>I am the parent</h1>
        { /* change code below this line */ }

        <ChildComponent />

        { /* change code above this line */ }
      </div>
    );
  }
};

<!-- 10 -->

const TypesOfFruit = () => {
  return (
    <div>
      <h2>Fruits:</h2>
      <ul>
        <li>Apples</li>
        <li>Blueberries</li>
        <li>Strawberries</li>
        <li>Bananas</li>
      </ul>
    </div>
  );
};

const Fruits = () => {
  return (
    <div>
      { /* change code below this line */ }
        <TypesOfFruit />
      { /* change code above this line */ }
    </div>
  );
};

class TypesOfFood extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        { /* change code below this line */ }
            <Fruits />
        { /* change code above this line */ }
      </div>
    );
  }
};


<!-- 11 -->

class Fruits extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h2>Fruits:</h2>
        { /* change code below this line */ }
          <NonCitrus />
          <Citrus />
        { /* change code above this line */ }
      </div>
    );
  }
};

class TypesOfFood extends React.Component {
  constructor(props) {
     super(props);
  }
  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        { /* change code below this line */ }
          <Fruits />
        { /* change code above this line */ }
        <Vegetables />
      </div>
    );
  }
};


<!-- 12 -->