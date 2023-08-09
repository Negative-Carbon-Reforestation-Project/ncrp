w![image](https://user-images.githubusercontent.com/28933557/173164536-108700d4-1676-48b0-9f01-20217052de0c.png)

#### Access our platform here: https://www.ncrp.app
## Introduction
We understand that technology cannot take the place of hands in the earth when it comes to reforestation efforts. However, we believe that it can serve to empower those involved.

For our capstone project, we developed a platform that utilizes convolutional neural networks and data science to identify potential locations for reforestation -- assisting those involved by reducing time and cost.

## Services

#### REST API

Our web application is built on top of a REST API that is available at the following endpoint:

``https://www.ncrp.app/maps/api/search/geo``

The endpoint expects two parameters, `longtitude` and `latitude`, and returns opportunities for reforestation and the tree species at the given coordinates.

For example:

`https://ncrp.app/api/search/geo?latitude=47.70023082782143&longitude=-123.58968272261251`

Returns the following json response:

```json
{
  "species": [
    {
      "wa_douglas_fir_stand_density": 0.08574207399322036,
      "wa_western_hemlock_stand_density": 0.11730453391478986,
      "wa_pacific_yew_basal_area": 0.036677908904923597
    }
  ],
  "wa_total_reforestation_opportunity": 0
}
```

#### Web Application

#### Accessibile at: https://www.ncrp.app

Our web application allows users to visualize and explore reforestation opportunities on a 2D and 3D map.

##### Visualization

We offer several base layers and landcover layers. The landcover layers were pre-processed by our data scientists.

[![Image from Gyazo](https://i.gyazo.com/faa03a908e2a921e610440f30806c627.gif)](https://gyazo.com/faa03a908e2a921e610440f30806c627)

Users are also able to visualize in 3D

[![Image from Gyazo](https://i.gyazo.com/f1d3198afabfd7fea25e6760ac7fe533.gif)](https://gyazo.com/f1d3198afabfd7fea25e6760ac7fe533)

##### Searching

To explore reforestation opportunities, users are able to place a marker on the map that makes requests to our REST API.

[![Image from Gyazo](https://i.gyazo.com/8a2407812f64d169c343a4e5d29c82b9.gif)](https://gyazo.com/8a2407812f64d169c343a4e5d29c82b9)

Alternatively, users are also able to search for locations directly using our search bar -- which supports auto-completion and geocoding.

[![Image from Gyazo](https://i.gyazo.com/7923e4f043e24df566ccef0edcdc4839.gif)](https://gyazo.com/7923e4f043e24df566ccef0edcdc4839)

## Contributors

#### Meet our amazing team

<table>
  <tr>
    <td align="center"><a href="https://github.com/asathkumara"><img src="https://avatars.githubusercontent.com/u/28933557?v=4?s=100" width="200px;" alt=""/><br /><sub><b>Asel S</b></sub></a><br />
    <td>
      <strong>Full-Stack Developer, UX-UI Designer</strong></br>
      <p>7+ years of full-stack development experience</p>
      <ul>
       <li>Developed web application using clean code practices in Node.js alongside JavaScript framework React.js and Redux to manage state</li>
        <li>Developed and structured REST API using Java, Maven and Spring framework</li>
        <li>Prototyped accessibile (WCAG 2.1 compliant), responsive and functional user interfaces for the web application to allow visitors on any device to have the same experience</li> 
        <li>Moderated usability / accessibility testing sessions for the desktop and mobile versions of the web application to identify bugs and improve overall user experience</li>
        <li>Conducted and converted data from UX survey, with 89 participants, into actionable points to further improve the user experience</li>
      </ul>
    </td>
  </tr>

  <tr>
    <td align="center"><a href="https://github.com/quicktkachuk"><img src="https://avatars.githubusercontent.com/u/59972585?v=4" width="200px;" alt=""/><br /><sub><b>Matthew Tkachuk</b></sub></a><br />
    <td>
      <strong>Back-End Developer, Data Scientist</strong></br>
      <p>Insert Summary</p>
      <ul>
        <li>Extended REST API functionality by implementing and configuring OpenSearch queries</li>
        <li>Data Science focus</li>
        <li>GIS data manipulation and preprocessing</li>
        <li>CNN Model design and construction</li>
        <li>CNN model training and hyperparameter manipulation</li>
      </ul>
    </td>
  </tr>

  <tr>
    <td align="center"><a href="https://github.com/liamstar97"><img src="https://avatars.githubusercontent.com/u/6600480?v=4" width="200px;" alt=""/><br /><sub><b>Liam Thompson</b></sub></a><br />
    <td>
      <strong>Cloud Engineer, Data Scientist, and ML Engineer</strong></br>
      <p>4+ years of cloud experience</p>
      <ul>
        <li>Designed backend architecture</li>
        <li>Deployed and maintained services on Kubernetes</li>
        <li>Deployed and configured services on Kubernetes</li>
        <li>Collected and analyzed data too predict reforestation opportunity</li>
        <li>Trained, deployed, and served Convolutional Neural Network to Ray cluster on k8s</li>
      </ul>
    </td>
  </tr>

  <tr>
    <td align="center"><a href="https://github.com/kylewhite0225"><img src="https://avatars.githubusercontent.com/u/66845776?v=4" width="200px;" alt=""/><br /><sub><b>Kyle White</b></sub></a><br />
    <td>
      <strong>React.js Developer, Data Scientist</strong></br>
      <p>4 years of aerospace manufacturing engineering experience, 
      2 years of cumulative experience in full-stack software development</p>
      <ul>
        <li>Developed query menu component and associated sub-components using JavaScript framework React.js, data visualization library Chart.js, and CSS</li>
        <li>Developed Python script to access US Forest Service ArcGIS REST API for downloading WA native tree species dataset</lI>
        <li>Developed Python based automation scripts for conversion of GeoTIFF data into point-lat/long coordinate CSV</li>
        <li>Used the above script to create an ArcGIS Pro script tool with parameterized inputs</li>
        <li>Assisted in optimization of hyperparameters of convolutional neural network reforestation prediction toolset</li>
        <li>Commissioned logo for website and branding</li>
        <li>Wrote about and mission statement excerpts</li>
      </ul>
    </td>
  </tr>
</table>


#### We'd like to credit the following people for helping us realize our project

<ul>
    <li>Seattle Sims for designing our amazing logo. You can view her portfolio here <a href="https://www.instagram.com/seattleasdesign/" target="_blank">https://www.instagram.com/seattleasdesign/</a></li>
    <li>Nancy Lane and Sara Farag for hosting our UX survey</li>
    <li>Liam's step-dad, Jake Mannix, for consulting with us on AWS and Machine Learning matters</li>
    <li>Alfred Nehme for advising our capstone group</li>
</ul>
