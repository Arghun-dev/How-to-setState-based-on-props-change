# How-to-setState-based-on-props-change

### to update state conditionally based on props change use componentDidUpdate lifecycle method:


```
componentDidUpdate(prevProps, prevState) {
    if (prevProps.MsgIdAuth !== this.props.MsgIdAuth) {
      if (this.props.MsgIdAuth === -1) {
        this.setState({
          alertType: 'danger',
          alertText: this.props.MsgTextAuth
        })
        console.log('rendered')
      }
    }
  }
```

