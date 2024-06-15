# prueba1
prueba de creacion de repositorio

print("hola")

meme_dict = {
    "LOL": "una respuesta a algo gracioso",
    "CRINGE": "algo raro o embarazoso",
    "ROFL": "una respuesta a una broma",
    "SHEESH": "ligera desaprobación",
    "CREEPY": "aterrador, siniestro",
    "AGGRO": "ponerse agresivo/enojado",
}

word = input("Escribe una palabra que no entiendas (¡con mayúsculas!): ").strip().upper()

if word in meme_dict:
    # Si se encuentra la palabra, mostramos su definición
    print(f'La palabra "{word}" significa: {meme_dict[word]}')
else:
    # Si no se encuentra la palabra, indicamos que no está en el diccionario y preguntamos si se quiere agregar
    print(f'La palabra "{word}" no se encuentra en el diccionario.')
    add_word = input("¿Quieres agregar esta palabra al diccionario? (sí/no): ").strip().lower()
    if add_word == 'sí':
        meaning = input("Introduce el significado de la palabra: ").strip()
        meme_dict[word] = meaning
        print(f'La palabra "{word}" ha sido añadida al diccionario con el significado: {meaning}')
