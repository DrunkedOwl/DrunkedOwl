- 👋 Hi, I’m @DrunkedOwl
- I’m interested in sharing and researching code for various purposes 👀  
- 🌱 I’m currently learning how to code WEB, and already know and have some experience in java, c, js, python, html, php and css
- 📫 How to reach me.
idk, just send a dm.

<!---
DrunkedOwl/DrunkedOwl is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

also look, I did a palindrome detector, kinda janky in some ways, but hey, I did it myself and I'm kinda proud of it

#include <stdio.h>
#include <string.h>
int main()
{
	//variables
	char cadena[25], cadena2[25];
	int pos, inver=0, cont=25, salir=0, carac, si=0, no=0;
	
	//recogida de datos
	printf("Dame la frase \n");
	fgets(cadena,25,stdin);
	carac=strlen(cadena);
	
	//eliminador de espacios
	for(pos=0; pos<=carac; pos++)
	{
		if(cadena[pos]!=' ')
		{
			cadena2[inver]=cadena[pos];
			inver++;
		}
			else
			{
				
			}
	}
	puts(cadena2);
	
    //Ciclo de comprobación
	carac=strlen(cadena2)-2;
	
		for(pos=0, inver=carac; pos<=carac, inver>=0; pos++, inver--)
        {

            printf("%c \n", cadena2[pos]);
            printf("%c \n", cadena2[inver]);

        	if(cadena2[pos]==cadena2[inver])
        	{
        		printf("coincidencia\n");
                si++;
			}
        	else
			{
				printf("Disparidad\n");
                no++;
			}
		}
        
        //respuesta
        if (si>no)
        	{
			printf("La frase es un palindromo \n");
			}
			else 
			{
        	printf("La frase no es un palindromo \n");
			}				
return 0;
}
