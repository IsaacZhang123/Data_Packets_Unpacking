
typedef struct
{
  U64 Head;
  U32 Command;
  U32 Para;
  U32 Sum
}Pack_T;
Pack_T mypack;

void SendPack()
{
  int i;
  U8* ptr8=(U8*)&mypack;
 for(i=0;i<sizeof(mypack);i++)
  {
     UartSend(*ptr8);//串口发送，不一样的库，函数不一样，或者自己实现
     ptr8++;
  }
}
