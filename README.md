Jupyter Images

Folder structure
/course
/docker-images
  /jupyter
  
1. Notebook
## always start from /jupyter folder to read toke information (do not use -d detached)
docker-compose up 

It will start the Jupyter Notebook 
anaconda_dev  | [C 22:39:20.180 NotebookApp] 
anaconda_dev  |     
anaconda_dev  |     To access the notebook, open this file in a browser:
anaconda_dev  |         file:///root/.local/share/jupyter/runtime/nbserver-1-open.html
anaconda_dev  |     Or copy and paste one of these URLs:
anaconda_dev  |         http://9de68738def0:8888/?token=bb1206f492ff34ce7d0ee7e03baa06718cb47e3436f9f892
anaconda_dev  |      or http://127.0.0.1:8888/?token=bb1206f492ff34ce7d0ee7e03baa06718cb47e3436f9f892

Open this link in your browser and expose /course folder