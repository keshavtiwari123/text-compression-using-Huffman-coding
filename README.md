# text-compression-using-Huffman-coding
To encode a text file, first you need to compile encode.cpp and huffman.cpp then link the object files together to make an exicutable file. To do this,
g++ encode.cpp huffman.cpp -o main
This will give a main file, now you need to run the main file to compress any file.
Suppose you need to compress a file call "TheInputFile.txt", to do this
./main TheInputFile.txt outputCompressesFile.huf
This will create a new file called "outputCompressesFile.huf"
Now this "outputCompressesFile.huf" will have smaller size than "TheInputFile", and it can be decompressed into original file
To decompress first you need to compile decode.cpp and huffman.cpp then link the object files together to make an exicutable file. To do this,
g++ decode.cpp huffman.cpp -o main
This will give an executable main file
To decompress a .huf file
Run ./main OutputCompressFile.huf OriginalFile.text
This will ceate a text file called OriginalFile.text which will contain the contents to original file.
