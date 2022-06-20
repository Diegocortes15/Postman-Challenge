# Postman Challenge
## Tutorial to run Postman Collection
### Prerequisites

#### Node.js

1. You need must have [Node.js](https://nodejs.org/en/) installed (Node.js LTS version recommended)
2. When you are installing Node.js, make sure to check the option

    - [x] **Automatically install the necesary tools. Note that this will also install Chocolatey. The script will pop-up in a new window after the installation completes.**

![nodeInstall](https://user-images.githubusercontent.com/60171460/157139770-d00bb969-9b36-4179-9dd2-ec5bf3fbd89a.PNG)

#### Newman and Newman reporter htmlextra

The easiest way to install Newman is using NPM. If you have Node.js installed, it is most likely that you have NPM installed as well.

> To run the following commands you have to open the ``` Command Promt ```.

![ezgif com-gif-maker (6)](https://user-images.githubusercontent.com/60171460/173421546-2e45537a-be5c-4feb-9222-e1d54bb0aab1.gif)

##### Intall ``` newman ```
``` 
npm install -g newman 
```

##### Intall ``` newman-reporter-htmlextra ```
```
npm install -g newman-reporter-htmlextra
```

## Download or Clone Repository

### Download

1. Click on the code button in this repository
2. Select the Download Zip option
3. Extract the .zip file with the **Extract here** option
4. Place the project folder on the desired location

### Clone

> Head to the folder when you would like clone the repository and run the following command

```
git clone https://github.com/Diegocortes15/Postman-Challenge.git
```

## Running project

1. In your Terminal, head to the folder where you saved the ``` .json ``` file.

![Capture (1)](https://user-images.githubusercontent.com/60171460/173421711-f6ba21fe-c583-4fdd-ba8d-a307673415a6.png)

2. Once there, run the following command to generate the report.

```
newman run SwaggerPetstoreAPI_collection.json -r htmlextra --reporter-htmlextra-browserTitle "SwaggerPetStore API Report" --reporter-htmlextra-export ./SwaggerPetstoreAPI_Reports/SwaggerPetStore-API-Report.html
```

## Open report

> Take in mind that you have to be in the folder where you have placed the .json file to run the following commands.

1. With the Terminal

  In your Terminal

  ```
  cd SwaggerPetstoreAPI_Reports
  ```

  Then,

  ```
  start SwaggerPetStore-API-Report.html
  ```
  
  ![ezgif com-gif-maker (5)](https://user-images.githubusercontent.com/60171460/173420598-a21eee59-c037-47af-a3ff-cf4173696480.gif)

  
2. With Windows interface

  - Open the folder ``` SwaggerPetstoreAPI_Reports ``` that has been created by ``` newman ``` plugin.
  - Open the ``` SwaggerPetStore-API-Report.html ``` file to show the **Swagger Pet Store API** report.

![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/60171460/173417648-2a26e612-8ccd-4079-a2b5-d123f784a57d.gif)
