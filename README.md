# Postup jak přidat další objekt:
## 1. vytvořit soubor [object]buffer.h a [object]buffer.cpp
- obsah udělat podobně jako např v spaceshipbuffer.h/.cpp
- v [object]buffer.c si v init() definovat body (můžete si pomoct s geogebrou)
- body spojit pomocí indices

## 2. vytvořir soubor [object]object.h/cpp
- do .cpp vykopírovat obsah z funkčního *object.cpp
- mění se spojení bodu (program->setAttributeBuffer(...))
- do .h zkoupírovát --||--, nezapomenout na include graphicalobject.h !

## 3. #include [object]object.h a [object]buffer.h do OpenGLScene.h

## 4. v OpenGL.cpp:
- si vytvořit nový buffer pro náš nový objekt
- do něj si .push_back instanci objektu
- [optional] pro náš objekt si vytvořit novy m_objects v .h(udělat nový for cyklus)
