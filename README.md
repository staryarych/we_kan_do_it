# we_kan_do_it

## Микрогайды для запуска АЙПУМБАХУЮМБА на kaggle
### Links:
    - https://www.kaggle.com/docs/api
    - https://github.com/Kaggle/kaggle-api/wiki/Kernel-Metadata#contents
### Конфиг    
    kaggle.json - получить в настройках kaggle

    ```bash   
        > mkdir /.kaggle
        > mv path/to/your/config/kaggle.json /.kaggle
        > mv /.kaggle /root/
        > chmod 600 ~/.kaggle/kaggle.json
        > ls ~/.kaggle/kaggle.json
    ```    
### Команды kaggle api  

    Надеюсь понятно, что где по структуре, я специально оставил свои конфиги

    Эти две генерят ваш конфиг для датасета\нотабукука, их надо будет поправить,
    !но можно просто поменять имя в моём, тогда можно скипать, они не как в git, доп мета не будет
    ```console    
         > kaggle kernels init -p path/to/dir/with/notebook
    ```   
    ```console    
         > kaggle datesets init -p path/to/dir/with/data
    ```   

    пуш = сохранить версию + запустить её с сохранение output файлов, которые потом можно забрать с каггла (веса и тд, главное сохранять их в коде)
    
    ```console    
        > kaggle kernels push -p path/to/metadata_file
    ```    
    ```console    
        > kaggle datasets version -p /path/to/dataset -m "Your message here"
    ```    
    
    мб мы там что-то, так что можно расширить наш датасет, просьба, тащить прошлые файлы, чтобы в версии и ваше 
    было и наше
    
    ```console    
        > kaggle datasets create -p path/to/metadata_file -u
    ```    
    
    
    и про подтянуть датасеты
    ```console
        > kaggle datasets download "nikitamalcev99/input-gpt2-kan"
        > unzip input-gpt2-kan.zip
    ```
