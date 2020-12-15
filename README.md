# **FRONT END JUNIOR TECHNICAL TEST FOR GUANE ENTERPRISES.**

## The test aims to create some functionalities based on the api hosted at https://tt.guane.com.co/api/loads, said test is made with HTML, CSS and VUEJS. A continuacion el resultado final.


![! ERROR Image does not load.](https://github.com/juliancastanedaDev/GUANE_enterprises/blob/main/images/image.png?raw=true)

# **USED ​​LANGUAGES**

- HTML
- CSS
- VUEJS


# **BLOQ PICKUP AND DELIVERY.**

## This block is programmed with HTML, CSS AND VUEJS, the data in the views zip_from, city_from, zip_to and city_to is extracted from the api shared by GUANE-enterprises.

![! ERROR Image does not load.](https://github.com/juliancastanedaDev/GUANE_enterprises/blob/main/images/image_1.png?raw=true)


# **BLOQ ACCESSORIALS.**

## This block is programmed with HTML, CSS AND VUEJS, the data in the views accessorials is extracted from the api shared by GUANE-enterprises, This block contains a checkbox section made in HTML and CSS.

![! ERROR Image does not load.](https://github.com/juliancastanedaDev/GUANE_enterprises/blob/main/images/image_2.png?raw=true)


# **BLOQ COMMODITY.**

## This block is programmed with HTML, CSS. This block contains two buttons to delete and create a new row, a table made with HTML and CSS and within the table a swift-type checkbox made with HTML and CSS.

![! ERROR Image does not load.](https://github.com/juliancastanedaDev/GUANE_enterprises/blob/main/images/image_3.png?raw=true)

# **CODE TO CONNECT TO API.**

Next I present the code used to bring the data and use it in my views, the VUEJS framework is used.

`<script>
                var urlApi = 'https://tt.guane.com.co/openapi.json'; 
                new Vue({
                    el: "#app",
                    created: function() {
                        this.getInfo();
                },
                data: {
                    lists : []
                },
                methods: {
                    getInfo: function() {
                        this.$http.get(urlApi).then(function(response){
                            this.lists = response.data.components.schemas.Hauls.properties;
                        });
                        }
                    }
                });
 </script>`      


# **WORK PREPARED BY**
_Julian Castañeda for GUANE-enterprises_
