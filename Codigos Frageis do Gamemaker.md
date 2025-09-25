//MUITO CUIDADO! ESSES CÓDIGOS NÃO PODEM SOFRER MUITAS ALTERAÇÕES! SE NÃO PODEM ACABAR NÃO FUNCIONANDO CORRETAMENTE

//ANDAR PARA OS LADOS DIREITO E ESQUERDO

if teclado_check(ord("D"))
{
x + = velocidade
x+=1
imagem_xscale=5
}
if teclado_check(ord("A"))
{
x -=velocidade
x-=1
imagem_xescala=-5
}

//COLISÇÃO E PULO

if place_meeting(x,y,Obj_wall)
{
   vvelocidade=0
   
   se teclado_check_pressionado(vk_space) && place_meeting(x,y+1,Obj_wall)
   {
    vvelocidade=-3
   }
}
outro
{
   vvelocidade+=0,3
}
//MUDAR AS "ANIMATIONS" NO CASO OS SPRITES DO PERSONAGEM 
//ESSES CÓDIGOS AINDA NÃO FORAM TERMINADOS

var num = skeleton_animation_get_frames(skeleton_animation_get());
image_index = num -1;
image_speed = 0;

