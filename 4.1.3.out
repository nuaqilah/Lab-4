#include<stdio.h>
#include<unistd.h>
#include<string.h>
#include<sys/socket.h>
#include<arpa/inet.h>     //inet_addr
@@ -18,7 +19,7 @@ int main(int argc,char*argv[])

    server.sin_addr.s_addr=inet_addr("110.159.160.109");
    server.sin_family=AF_INET;
    server.sin_port=htons(22);
    server.sin_port=htons(8888);

    //Connect to remote server
    if(connect(socket_desc,(struct sockaddr*)&server,sizeof(server))<0)
@@ -44,5 +45,6 @@ int main(int argc,char*argv[])
    puts("Reply received\n");
    puts(server_reply);

    close(socket_desc);
    return 0;
}
