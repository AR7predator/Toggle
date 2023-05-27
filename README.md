# Toggle

import React, { useState } from 'react';

const App = () => {
  const [backgroundColor, setBackgroundColor] = useState('white');

  const toggleBackgroundColor = () => {
    setBackgroundColor(backgroundColor === 'white' ? 'lightblue' : 'white');
  };

  return (
    <div style={{ backgroundColor }}>
      <h1>Toggle Background Color</h1>
      <button onClick={toggleBackgroundColor}>Toggle</button>
    </div>
  );
};

export default App;
