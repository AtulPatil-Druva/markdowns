The orion button component can be used to display the following types of buttons:
![alt text](image.png)

Import the button component this way:
```javascript
import Button from "orion/lib/button";

```
| Property       | Data Type                   | Default Value   | Description                                                                                                                                                                                                                             |
|----------------|-----------------------------|-----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `label`        | String                     | -               | The label of the button.                                                                                                                                                                                                               |
| `type`         | String                     | secondary       | Type of the Button component. Can be either "primary", "secondary", "danger" or "link".                                                                                                                                                 |
| `isSuccess`    | Boolean                    | false           | If passed as true, the button will be shown in success color. We could not take it in type prop because then outline variant of success was not possible. Now if you pass isSuccess with primary and secondary type, it will be shown as filled and outlined buttons respectively. |
| `size`         | String                     | md              | Size of the Button component. Can be either "sm", "md" or "lg". Font size, padding will be automatically adjusted.                                                                                                                      |
| `href`         | String                     | -               | `href` is required for link button only. If `href` is provided then the button is created using `<a>` else using `<button>`.                                                                                                             |
| `icon`         | `<FromOrionIconsLibrary />`| -               | **Icon React Element** imported from orion-icons library. If you want the icon color changed on hover of the button, please pass `inheritFontColor` prop to the Icon component.                                                          |
| `disabled`     | Boolean                    | false           | Handles the disability of the button.                                                                                                                                                                                                  |
| `active`       | Boolean                    | false           | Makes button style look active.                                                                                                                                                                                                        |
| `block`        | Boolean                    | false           | Full-width button.                                                                                                                                                                                                                     |
| `onClick`      | Function                   | -               | Click handler function for the button.                                                                                                                                                                                                 |
| `onMouseDown`  | Function                   | -               | Mouse down handler function for the button.                                                                                                                                                                                            |
| `onMouseUp`    | Function                   | -               | Mouse up handler function for the button.                                                                                                                                                                                              |
| `className`    | String                     | -               | Provision to pass custom class.                                                                                                                                                                                                        |
| `dataTestId`   | String                     | orion-button    | Provision to pass a custom data test ID for automation purposes.                                                                                                                                                                       |


How to use the Button component for different use cases?

1. Primary Button- This is a blue colored button  
![alt text](image-1.png)
```javascript
<Button label="primary" type="primary"/>
```
2. Secondary Button- This is a white colored button. Secondary is the default type  
![alt text](image-2.png)
```javascript
<Button label="secondary" type="primary"/>
```
3. Danger Button - This is a red colored button  
![alt text](image-3.png)
```javascript
<Button label="danger" type="danger"/>
```
4. Link Button- This is a button component but displayed like a link  
![alt text](image-4.png)
```javascript
<Button label="link button" type="link" href="/dummylink"/>
```

Button states can be disabled which is handled by the 'disabled' prop.

Button sizes are handled by the size prop






