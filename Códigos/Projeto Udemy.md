

# Background movimento para direita

- Habilitar Horizontal tile
- Velocidade horizontal = Valor x 


# room
if (room == Room3)
{

room_goto(room1)
}

else

{
room_goto_next();
}



-  Novos layers para objetos de itens ou coisas que necessáriamente tem que ficar em cima


draw_set_font(Font1);
draw_set_halign(fa_center);
draw_set_valign(fa_middle);

draw_text(x, y, botao_texto);

draw_set_halign(fa_left);
draw_set_valign(fa_top);


// Pontuação
draw_text(10,10, "Pontos: " + string(global.pontuacao));

// Recorde
draw_text(10,30, "Recorde: " + string(global.recorde));

// Vidas
draw_text(room_width - 100, room_height - 30, "Vidas: " + string(global.vidas));

