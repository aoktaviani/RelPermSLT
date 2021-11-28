# RelPermSLT
JScript source code to generate the SLT table using the Corey equation
// JScript source code to generate the SLT table using the Corey equation
var Slcon=Swcon+Soirg;
var Slrg=Swcon+Sorg;
var slmin=Slcon;
var slmax=1-Sgcon;
var kwlines="**$ SL krg krog";
var sl=slmin;
var krg, krog;
while(sl<=slmax+0.000001)
{
if(sl<=Slrg)
{krog=0; }
else
{ krog=Krogcg*Math.pow((sl-Slrg)/(1-Sgcon-Slrg),nog);}
var next Sl=sl+0.01;
if(sl>1-Sgcrit|| nextSl>slmax+0.000001)
{krg=0;}
else
{ krg=Krgcl*Math.pow((1-Sgcrit-sl)/(1-Sgcrit-Slcon),ng);}
kwlines+="\r\n"+" "+sl.toFixed(3)+" "+krg.toFixed(8)+" "+krog.toFixed(8);
sl=sl+0.01;
}
kwlines;
