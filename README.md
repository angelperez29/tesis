# Repositorio en el que se almacenarán los notebooks y códigos la tesis

### @Author Florentino Ángel Pérez Arce

- Para instalar marisa-trie (dependencia para spanish_sentiment_analysis), es necesario descargar la biblioteca y sus códigos fuente desde github dado que la herramienta pip no logra instalarlo (al menos hasta la versión 0.7.5) de manera correcta por lo que debemos ejecutar el siguiente comando:
· git clone https://github.com/pytries/marisa-trie.git && cd marisa-trie && rm -r marisa-trie && pip install --no-cache-dir cython && ./update_cpp.sh && git clone https://github.com/s-yata/marisa-trie.git && python setup.py install

Lo que hace es:
    - Clonar el repositorio de la biblioteca
    - Eliminar el directorio marisa-trie en la cual se supondría se almacenarían los códigos fuente
    - Instalamos cython, necesario para la construcción de la biblioteca
    - Actualizamos los ficheros
    - Clonar el codigo fuente de marisa-trie 
    - Y finalmente instalar la biblioteca
