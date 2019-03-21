---
title: Example Post
date: "2018-03-21"
description: Something Something Description
---

This is an example placeholder post to show how to do different things in markdown.

```jsx
const StoreContext = React.createContext();

class StoreProvider extends Component {
  constructor(props) {
    super(props);

    this.state = {
      user: 'Me'
    }
  }

  render() {
    return (
      <StoreContext.Provider
        value={{
          state: this.state,
        }}
      >
        {this.props.children}
      </StoreContext.Provider>
    );
  }
}

export const StoreConsumer = StoreContext.Consumer;

export default StoreProvider;
```