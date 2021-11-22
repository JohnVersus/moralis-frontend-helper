# `moralis-frontend-helper`
> Part of Moralis weekly challenge 

> The main aim of this project is to make the the frontend development easy with **Moralis** for anyone with very basic knowledge of programming / NoCoders / LowCoders.

## Setup:

## With the help of moralis-frontend-helper:
1. User will be able to inject working moralis functions directly into their web page.  
2. Get HTML code instantly by running moralis-frontend-helper function which later can be used to add to any of their HTML code. 
3. Gives user ability to give custom styling to their webpage.  

# UI Element Functions which uses moralis web3api functions

- [`addTokenSelect()`](#addTokenSelect)
  - **`Adds a dropdown into the page with token names`**
  - `The below code creates a dorpdown select in document with element id = Select1, inside parent element of id = Body, with default dropdown = Select and with styling text alignment = center, text color = #000000. **And most importantly it gets the token names from Uniswap and Pancake swap and adds it to the dropdown select**`
 
    ```
    options = {
    TagID:"Select1", ParentId:"Body", DefaultValue:"Select", Style:"text-align: center; color: #000000;"
    }
    addTokenSelect(options)
    ```

- [`AddLoginButton()`](#AddLoginButton)
  - **`Adds a Metamask login button element into the page`**
  - `The below code adds an button element into the document with element id = LoginBtn, inside parent element of id = Body, with height = 15px and width = 50px and Background color = #65a47b . **And can be used to login into metamask wallet.**`
 
    ```
    options = {
    TagID:"LoginBtn", ParentId:"Body", Style:"min-width: 50px; min-height: 15px; background-color: #65a47b;"
    }
    AddLoginButton(options)
    ```

- [`AddWCLoginButton()`](#AddWCLoginButton)
  - **`Adds a Wallet Connect login button element into the page`**
  - `The below code adds an button element into the document with element id = LoginBtn, inside parent element of id = Body, with height = 15px and width = 50px and Background color = #65a47b . **And can be used to login into crypto wallets using Wallet Connect funtions.**`
 
    ```
    options = {
    TagID:"LoginBtn", ParentId:"Body", Style:"min-width: 50px; min-height: 15px; background-color: #65a47b;"
    }
    AddLoginButton(options)
    ```

- [`AddButton()`](#AddButton)
  - **`Adds a button element with moralis web3api functions into the page`**

    **Accepted Button Function**
    - Login `Requies no input elememt, requires output text element to store user address`
    - Logout `Requies no input elememt, requires no output element`
    - Balance `Requies input element with wallet address, requires output table element with two columns ["Address", "Balances"]`
    - Transaction `Requies input element with wallet address, requires output table element with five columns ["Chanin", "From Address", "To Address", "Value", "Transaction Date"]`
    - NFT `Requies input element with text element to search  for NFT, requires output div element to store search output`
    - TokenPrice `Requies input element with token contract address, requires output text element to show price`
    
  - `The below code adds an button element into the document with element id = Button1, inside parent element of id = Body, with button onclick function as to get token price which takes input from the UI element = Intext1 and sends output into an UI element Text1 with height = 15px and width = 50px and Background color = #65a47b . **And can be used to login into crypto wallets using Wallet Connect funtions.**`
 
    ```
    options = {
    TagID:"Button1", ParentId:"Body", ButtonName:"ClickMe", ButtonFunction:"TokenPrice", FunctionInput:"InText1", FunctionOutput:"Text1", Style:"min-width: 50px; min-height: 15px; background-color: #65a47b;"
    }
    AddButton(options)
    ```


# UI Element Functions
- [`addText()`](#addText)
  - **`Adds a UI text element to the page`**
  - `The below code creates a text element in document with element id = Text, inside parent element of id = Body, with text value = Hello World!!, text color = #000000 .`
 
    ```
    options = {
    TagID:"Text", ParentId:"Body", Text:"Hello World!!", Style:"color: #000000;"
    }
    addText(options)
    ```
    
- [`createDiv()`](#createDiv)
  - **`Adds an div element into the page`**
  - `The below code adds an div element into the document with element id = Div1, inside parent element of id = Body, with height and width = 100px and Background color = #8765d5 .`
 
    ```
    options = {
    TagID:"Div1", ParentId:"Body", Style:"min-width: 100px; min-height: 100px; background-color: #8765d5;"
    }
    createDiv(options)
    ```

- [`createRowDiv()`](#createRowDiv)
  - **`Adds an div element into the page which flexes as row`**
  - `The below code adds an div element which flexes as row into the document with element id = Row1, inside parent element of id = Body, with height and width = 100px and Background color = #8765d5 .`
 
    ```
    options = {
    TagID:"Row1", ParentId:"Body", Style:"min-width: 100px; min-height: 100px; background-color: #8765d5;"
    }
    createRowDiv(options)
    ```

- [`createColumnDiv()`](#createColumnDiv)
  - **`Adds an div element into the page which flexes as column`**
  - `The below code adds an div element which flexes as column into the document with element id = Colm1, inside parent element of id = Body, with height and width = 100px and Background color = #8765d5 .`
 
    ```
    options = {
    TagID:"Colm1", ParentId:"Body", Style:"min-width: 100px; min-height: 100px; background-color: #8765d5;"
    }
    createColumnDiv(options)
    ```

- [`AddInputTextBox()`](#AddInputTextBox)
  - **`Adds a UI input text element to the page`**
  - `The below code creates a input text element in document with element id = InText, inside parent element of id = Body, with Placeholder value = Enter Text, text color = #000000 .`
 
    ```
    options = {
    TagID:"InText", ParentId:"Body", Placeholder:"Enter Text", Style:"color: #000000;"
    }
    AddInputTextBox(options)
    ```
    
- [`CreateTable()`](#CreateTable)
  - **`Adds a table into the page`**
  - `The below code creates a table in document with element id = Table1, inside parent element of id = Body, with columns = Colm1, Colm2, Colm3  and with styling text alignment = center, text color = #000000 .`
 
    ```
    options = {
    TagID:"Table1", ParentId:"Body", ColumnNames:["Colm1", "Colm2", "Colm3"], Style:"text-align: center; color: #000000;"
    }
    CreateTable(options)
    ```

- [`addImage()`](#addImage)
  - **`Adds an image into the page`**
  - `The below code adds an image into the document with element id = Image1, inside parent element of id = Body, with image from "https://picsum.photos/id/237/200/300" and with  Background color = #000000 .`
 
    ```
    options = {
    TagID:"Image1", ParentId:"Body", Image:"https://picsum.photos/id/237/200/300", Style:"background-color: #000000;"
    }
    addImage(options)
    ```

- [`DeleteDiv()`](#DeleteDiv)
  - **`Deletes UI element from the page.`**
  - `The below code deletes a element with id= Text from page .`
 
    ```
    DeleteDiv("Text")
    ```
    
- [`DeleteContent()`](#DeleteContent)
  - **`Removes the content that is present in a UI element.`**
  - `The below code removes the content that is present in a UI element with id= "Text" .`
 
    ```
    DeleteContent("Text")
    ```




