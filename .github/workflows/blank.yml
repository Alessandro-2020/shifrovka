def shifrovka (word, key):
        result = ''
        for l,k in zip(word, key):
                new_l = ord(l)+(ord(k)-ord("A"))
                if new_l>90:
                    new_l-=26
                    
                result += chr(new_l)
        return result
def deshifrovka (word, key):
    result = ''
    for l,k in zip(word, key):
            new_l = ord(l)-(ord(k)-ord("A"))
            if new_l<65:
                new_l+=26
                    
            result += chr(new_l)
    return result
def kluch(word, key):
        size_word = len(word)
        while len(key) < size_word:
                key += key
        return key
 
dct = {}
start, end = ord('a'), ord('z')+1
for i in range(start, end):
        dct[chr(i)] =  i - start
a = input('0=шифровка, 1=расшифровка:')               
word = input('Введите слово(большими буквами):  ')
key = input('ключ(большими буквами):  ')
new_key = kluch(word, key)
if a==0:
   print ('Зашифрованное слово:', shifrovka (word, new_key))
else:
   print ('Расшифрованное слово:', deshifrovka (word, new_key))

