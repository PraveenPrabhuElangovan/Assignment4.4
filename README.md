1) Java program to copy a file from HDFS to LFS;
  I attached screenshot for the above program
  
  
2)Explain the importance and usage of the below terms in details
DFSInputStream 
• Handles communication of the namenode with various datanodes. 
• Handles integrity of data contained by the blocks. 
• Manages data read activity in case of datanode failure. 
• Called internally by FSDataInputStream. 
DFSOutputStream
• Handles communication of the namenode with various datanodes. 
• Called internally by FSDataOutputStream.
FSDataInputStream
FSDataInputStream wraps the DataInputStream and implements Seekable, PositionedReadable interfaces which provide method like getPos(), seek() method to provide Random Access on HDFS file.
Below sample code uses seek (), getPos () and read() method FSDataInputStream also implements PositionedReadable
FSDataOutputStream
 • Provides stream (channel) for writing data. Filesystem’s create () method return FSDataOutputStream, which use to create new HDFS file or write the content at the EOF.
