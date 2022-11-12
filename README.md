# A simple react modal component library using `create-react-app`.

## Installation 

Run the following command:`npm install simple-modal-component`

## Getting Started with this modal component

The modal component accepts three props which are required:
> **message** prop which is used to display in the modal

> **isVisible** is taking a boolean value and will display the modal when the value is true

> **handleClose** is taking a callback function and will call this function from the modal when closing button is clicked or Esc is pressed

Here is an example of using modal with the help of useState hook:

``` 
export function Example() {

    const [displayModal, setDisplayModal] = useState(true);

    return (
        <Modal 
            isVisible={displayModal} 
            message={"write your message here!"} 
            handleClose={() => setDisplayModal(false)}
        />)
}

```

## Overwrite the style by using the differents css classes


> **modal-wrapper** for the layout of the modal (it constains the modal and the backdrop)

> **modal** for the modal card

> **modal-backdrop** for the background layer behind the modal
You can change the background-color using the property background-color

> **modal-message** for the style of the message

> **modal-closing** for the closing button



