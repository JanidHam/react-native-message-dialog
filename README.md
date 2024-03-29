# react-native-message-dialog

A simple, dialog message component with callback action like Airbnb. Ideal for showing errors, info and warnings.

![](assets/message-view.gif)


## Installation

If using npm:

```
npm i react-native-message-dialog
```

## Usage

```
import Message from 'react-native-message-dialog'
```

Simply place a `<Message />` inside of any compnent.

```
<View style={{ flex: 1 }}>
    <Message visible={true} />
</View>
```

### Styling Usage
Message is fully customizable using the `height, textStatus, textCb,  textMessage, textStatusStyle and textCbStyle` props.

Example usage to change dots color:

```
const textStatusStyle = {
    color: 'red',
};

return (
    <View style={{flex: 1}}>
        <Message visible={true} textStatusStyle={textStatusStyle} />
    </View>
)
```

## Documentation

### Message Component
| Name            | Description                                           | Default           | Type     |
|-----------------|-------------------------------------------------------|-------------------|----------|
| visible         | Determinates if message container is visible          | false             | Boolean  |
| onPress         | Callback to retry an action                           | () => ({})        | Function |
| textStatus      | Left text of the message container                    | Error             | String   |
| textCb          | Right text of the message container (Callback action) | Retry             | String   |
| textMessage     | Center text of the message container                  | Please try again. | String   |
| textStatusStyle | Style to apply to textMessage                         | Object            | Object   |
| textCbStyle     | Style to apply to textCb                              | Object            | Object   |

## Contributing
Pull requests are always welcome! Feel free to open a new GitHub issue for any changes that can be made.

## Author
Janid Ham | [https://janidham.com](https://janidham.com)

## License
[MIT](./LICENSE)

<style>.bmc-button img{width: 27px !important;margin-bottom: 1px !important;box-shadow: none !important;border: none !important;vertical-align: middle !important;}.bmc-button{line-height: 36px !important;height:37px !important;text-decoration: none !important;display:inline-flex !important;color:#ffffff !important;background-color:#FF813F !important;border-radius: 3px !important;border: 1px solid transparent !important;padding: 1px 9px !important;font-size: 22px !important;letter-spacing:0.6px !important;box-shadow: 0px 1px 2px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;margin: 0 auto !important;font-family:'Cookie', cursive !important;-webkit-box-sizing: border-box !important;box-sizing: border-box !important;-o-transition: 0.3s all linear !important;-webkit-transition: 0.3s all linear !important;-moz-transition: 0.3s all linear !important;-ms-transition: 0.3s all linear !important;transition: 0.3s all linear !important;}.bmc-button:hover, .bmc-button:active, .bmc-button:focus {-webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;text-decoration: none !important;box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;opacity: 0.85 !important;color:#ffffff !important;}</style><link href="https://fonts.googleapis.com/css?family=Cookie" rel="stylesheet"><a class="bmc-button" target="_blank" href="https://www.buymeacoffee.com/janidham"><img src="https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/BMC-btn-logo.svg" alt="Buy me a coffee"><span style="margin-left:5px">Buy me a coffee</span></a>