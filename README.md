# iv2021-M*yb*nk Assessment
**Language** = HTML, CSS, Javascript (jQuery & AJAX) <br />
**Front-end** = Bootstrap, chartJS, leafletJs <br /> 
**Back end/API** = nodeJS (npm package called `json-server` as fake API) & real-time API`https://api.wheretheiss.at/` <br /> 


# To install
**For front-end:** <br /> 
[1] Go to your local server directory (httpdocs dir for XAMPP) <br /> 
[2] Open terminal/git bash and type `git clone https://github.com/syukranDev/iv2021_syukran.git` <br /> 
[2] Fire up your local server. <br /> 

**For back-end:** <br /> 
**Assuming you have nodejs installed** <br /> 
[1] Go to path `iv2021_syukran/fakeAPI` and delete all files except `db.json` and make a copy of it to desktop (will use later in step 5) <br />
[2] Open terminal in `iv2021_syukran/fakeAPI` directory and type `npm install -D json-server` <br />
[3] Run the fakeAPI server by `json-server --watch db.json`, this if all good, your JSON server will be running at port 3000 (http://localhost:3000) <br /> 
[4] `node_modules` , `db.json`, `package.json`, `package-lock.json` will be generated. <br />
[5] Replace the `db.json` generated by the JSON server with the `db.json` you copied to desktop. <br />

<!-- ![1](https://user-images.githubusercontent.com/51852197/88816718-44360000-d1ef-11ea-933d-1b5e2ba762ae.PNG) -->
<!-- update this later, check again -->


# Web Apps Explanation
-**terminal tab 1 & 2 & 3 ==>** used self-generate data inside the `db.json`, all data shown in `db.json` is fetched (METHOD: GET) by jQuery/AJAX from `api-url: http://localhost:3000/Todos` (Todos is a parent name of db.json 's child content) <br />
-**terminal tab 4 (twiter) ==>** tweet ID is fetched manually by simply going to tweet url (https://twitter.com/username/status/tweetID). Planned to get new Twitter API token key to query (GET) the tweet ID, but application rejected. <br />
-**terminal tab 4 (how-many-people-in-space) ==>** data is fetch (GET) directly from `https://api.wheretheiss.at/` <br /> 


![webpage full](https://user-images.githubusercontent.com/51852197/144365761-77372233-c657-4fe5-9b20-6651a8c09178.png)


# Remarks & Future Dev
-`json-server` is a full fake REST API used for quick backend prototyping,  more infos here: https://www.npmjs.com/package/json-server <br />
-`db.json` of fakeAPI (json-server) only contain 11 sets of self-generate data (lattitude,longitude,temperature,country,id,timestamp) due to simplicity and most opensource api doesnt provides all these in one shot.  <br />
-not really meet the main task objective due to time constraint & limited knowledge on DOM manipulation, but i think meet the Extension A,B,C.



