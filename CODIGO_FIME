#include<stdio.h>
#include<stdlib.h>
int top=-1;
int tr[5];
int val=0;
void escoge();
void push(int);
int pop();
void display();
char nom[100];
int lun=0,mar=0,mie=0,jue=0,vie=0,lunh=0,marh=0,mieh=0,jueh=0,vieh=0;
int dia=0,hora=0,min=0,rep=0;

int main(){
	int option=0;
printf("***************************************MENU DE CAJAS FIME***************************************");
printf("\nIngrese su nombre: "); gets(nom);
printf("\nBienvenido %s al menu de cajas FIME, este programa tiene el fin de poder brindarle al usuario la oportunidad de reservar horarios para un espacio en la caja de FIME.",nom);
	do
    {
        printf("\n\nTendra la opcion de agregar cierta cantidad de turnos, solo puede agregar un turno por dia. En caso que desee eliminar el primer turno que asigno, debera eliminar primero los turnos posteriores que haya agregado.");
        printf("\nSe le mostrara las opciones que desea hacer con los turnos.");
		printf("\n1. Push/Agregar turno.");
        printf("\n2. Pop/Eliminar turno.");
        printf("\n3. Display/Visualizar turnos.");
        printf("\n4. Exit/Salir del menu.");
        printf("\nIngresa una opcion: ");
        scanf("%d", &option);
        switch(option)
        {
            case 1:
                escoge();
                push(val);
                break;
            case 2:
                val = pop();
                switch(val){
                	case 11: lun=0; lunh=0;
                	break;
                	case 12: lun=0; lunh=0;
                	break;
                	case 13: lun=0; lunh=0;
                	break;
                	case 14: lun=0; lunh=0;
                	break;
                	case 21: mar=0; marh=0;
                	break;
                	case 22: mar=0; marh=0;
                	break;
                	case 23: mar=0; marh=0;
                	break;
                	case 24: mar=0; marh=0;
                	break;
                	case 31: mie=0; mieh=0;
                	break;
                	case 32: mie=0; mieh=0;
                	break;
                	case 33: mie=0; mieh=0;
                	break;
                	case 34: mie=0; mieh=0;
                	break;
                	case 41: jue=0; jueh=0;
                	break;
                	case 42: jue=0; jueh=0;
                	break;
                	case 43: jue=0; jueh=0;
                	break;
                	case 44: jue=0; jueh=0;
                	break;
                	case 51: vie=0; vieh=0;
                	break;
                	case 52: vie=0; vieh=0;
                	break;
                	case 53: vie=0; vieh=0;
                	break;
                	case 54: vie=0; vieh=0;
                	break;
				}
                if(val != -1)
                    printf("\nEl turno eliminado es el numero %d", val);
                break;
            case 3:
                display();
                break;
        }
    }while(option != 4);


	return 0;
}

void escoge(){

	
	printf("\nSeleccione un dia que pueda asisitir a cajas, si no se encuentra el dia escriba el numero 0 para salir de esta opcion.");
	printf("\n1.-Lunes\n2.-Martes\n3.-Miercoles\n4.-Jueves\n5.-Viernes\n");
	do{printf("\nDigite un numero que represente alguno de los 5 dias: "); scanf("%d",&dia);} while(dia<0 && dia>5);
	if (dia>=1 && dia<=5){
		do{
			switch(dia){
				case 1: do{ printf("\nSe utilizara un sistema de 24 hrs.\nPor ejemplo, si desea ingresar el horario de las 3 pm, usted debe digitar el numero 15 (que representa a las 3 pm).\n");
				printf("\nDigite por favor el horario donde posee disponibilidad: "); scanf("%d",&hora);
				if(hora>=8 && hora<=19){ printf("\nLas cajas de FIME abren de 8:30 - 19:00. Por lo que es necesario que seleccione un horario disponible.");
				printf("\nIngrese porfavor un numero que representa el lapso del tiempo en donde tiene disponible: ");
				printf("\n1.- 0 a 15 minutos de la hora\n2.- 15 a 30 minutos de la hora\n3.- 30 a 45 minutos de la hora\n4.- 45 a 60 minutos de la hora\nDigite numero: "); scanf("%d",&min);
				if(hora==8 && min>=1 && min<=2){ printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario le invitamos a que regrese al menu para agregar su turno. Gracias por su comprension."); }
				else{ switch(min){ 
				      case 1: printf("\nUsuario %s su turno es el numero 11, empieza el dia Lunes a las %d:00 y termina a las %d:15.",nom,hora,hora); val=11; lun++; lunh=lunh+hora;
				      break;
				      case 2: printf("\nUsuario %s su turno es el numero 12, empieza el dia Lunes a las %d:15 y termina a las %d:30.",nom,hora,hora); val=12; lun++; lunh=lunh+hora;
				      break;
				      case 3: printf("\nUsuario %s su turno es el numero 13, empieza el dia Lunes a las %d:30 y termina a las %d:45.",nom,hora,hora); val=13; lun++; lunh=lunh+hora; 
				      break;
				      case 4: printf("\nUsuario %s su turno es el numero 14, empieza el dia Lunes a las %d:45",nom,hora); hora=hora+1; printf(" y termina a las %d:00.",hora); val=14; lun++; lunh=lunh+hora-1;
				      break;
				      default: printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario se le invita regresar al menu. Gracias por su comprension.");
				      break;
				      }
				}
				rep=0;} 
				else{ printf("\nLo sentimos, no se encuentran turnos disponibles a esta hora seleccionada. Si desea terminar de agregar, porfavor digite 0, en caso que desee escoger otro horario, digite cualquier otro numero y presione enter: "); scanf("%d",&rep); }
				} while(rep!=0);
					
					break;
				
				case 2: do{ printf("\nSe utilizara un sistema de 24 hrs.\nPor ejemplo, si desea ingresar el horario de las 3 pm, usted debe digitar el numero 15 (que representa a las 3 pm).\n");
				printf("\nDigite por favor el horario donde posee disponibilidad: "); scanf("%d",&hora);
				if(hora>=8 && hora<=19){ printf("\nLas cajas de FIME abren de 8:30 - 19:00. Por lo que es necesario que seleccione un horario disponible.");
				printf("\nIngrese porfavor un numero que representa el lapso del tiempo en donde tiene disponible: ");
				printf("\n1.- 0 a 15 minutos de la hora\n2.- 15 a 30 minutos de la hora\n3.- 30 a 45 minutos de la hora\n4.- 45 a 60 minutos de la hora\nDigite numero: "); scanf("%d",&min);
				if(hora==8 && min>=1 && min<=2){ printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario le invitamos a que regrese al menu para agregar su turno. Gracias por su comprension."); }
				else{ switch(min){ 
				      case 1: printf("\nUsuario %s su turno es el numero 21, empieza el dia Martes a las %d:00 y termina a las %d:15.",nom,hora,hora); val=21; mar++; marh=marh+hora;
				      break;
				      case 2: printf("\nUsuario %s su turno es el numero 22, empieza el dia Martes a las %d:15 y termina a las %d:30.",nom,hora,hora); val=22; mar++; marh=marh+hora;
				      break;
				      case 3: printf("\nUsuario %s su turno es el numero 23, empieza el dia Martes a las %d:30 y termina a las %d:45.",nom,hora,hora); val=23; mar++; marh=marh+hora;
				      break;
				      case 4: printf("\nUsuario %s su turno es el numero 24, empieza el dia Martes a las %d:45",nom,hora); hora=hora+1; printf(" y termina a las %d:00.",hora); val=24; mar++; marh=marh+hora-1;
				      break;
				      default: printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario se le invita regresar al menu. Gracias por su comprension.");
				      break;
				      }
				}
				rep=0;} 
				else{ printf("\nLo sentimos, no se encuentran turnos disponibles a esta hora seleccionada. Si desea terminar de agregar, porfavor digite 0, en caso que desee escoger otro horario, digite cualquier otro numero y presione enter: "); scanf("%d",&rep); }
				} while(rep!=0);
					
					break;
				
				
				case 3: do{ printf("\nSe utilizara un sistema de 24 hrs.\nPor ejemplo, si desea ingresar el horario de las 3 pm, usted debe digitar el numero 15 (que representa a las 3 pm).\n");
				printf("\nDigite por favor el horario donde posee disponibilidad: "); scanf("%d",&hora);
				if(hora>=8 && hora<=19){ printf("\nLas cajas de FIME abren de 8:30 - 19:00. Por lo que es necesario que seleccione un horario disponible.");
				printf("\nIngrese porfavor un numero que representa el lapso del tiempo en donde tiene disponible: ");
				printf("\n1.- 0 a 15 minutos de la hora\n2.- 15 a 30 minutos de la hora\n3.- 30 a 45 minutos de la hora\n4.- 45 a 60 minutos de la hora\nDigite numero: "); scanf("%d",&min);
				if(hora==8 && min>=1 && min<=2){ printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario le invitamos a que regrese al menu para agregar su turno. Gracias por su comprension."); }
				else{ switch(min){ 
				      case 1: printf("\nUsuario %s su turno es el numero 31, empieza el dia Miercoles a las %d:00 y termina a las %d:15.",nom,hora,hora); val=31; mie++; mieh=mieh+hora;
				      break;
				      case 2: printf("\nUsuario %s su turno es el numero 32, empieza el dia Miercoles a las %d:15 y termina a las %d:30.",nom,hora,hora); val=32; mie++; mieh=mieh+hora;
				      break;
				      case 3: printf("\nUsuario %s su turno es el numero 33, empieza el dia Miercoles a las %d:30 y termina a las %d:45.",nom,hora,hora); val=33; mie++; mieh=mieh+hora;
				      break;
				      case 4: printf("\nUsuario %s su turno es el numero 34, empieza el dia Miercoles a las %d:45",nom,hora); hora=hora+1; printf(" y termina a las %d:00.",hora); val=34; mie++; mieh=mieh+hora-1;
				      break;
				      default: printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario se le invita regresar al menu. Gracias por su comprension.");
				      break;
				      }
				}
				rep=0;} 
				else{ printf("\nLo sentimos, no se encuentran turnos disponibles a esta hora seleccionada. Si desea terminar de agregar, porfavor digite 0, en caso que desee escoger otro horario, digite cualquier otro numero y presione enter: "); scanf("%d",&rep); }
				} while(rep!=0);
					
					break;
				
				case 4: do{ printf("\nSe utilizara un sistema de 24 hrs.\nPor ejemplo, si desea ingresar el horario de las 3 pm, usted debe digitar el numero 15 (que representa a las 3 pm).\n");
				printf("\nDigite por favor el horario donde posee disponibilidad: "); scanf("%d",&hora);
				if(hora>=8 && hora<=19){ printf("\nLas cajas de FIME abren de 8:30 - 19:00. Por lo que es necesario que seleccione un horario disponible.");
				printf("\nIngrese porfavor un numero que representa el lapso del tiempo en donde tiene disponible: ");
				printf("\n1.- 0 a 15 minutos de la hora\n2.- 15 a 30 minutos de la hora\n3.- 30 a 45 minutos de la hora\n4.- 45 a 60 minutos de la hora\nDigite numero: "); scanf("%d",&min);
				if(hora==8 && min>=1 && min<=2){ printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario le invitamos a que regrese al menu para agregar su turno. Gracias por su comprension."); }
				else{ switch(min){ 
				      case 1: printf("\nUsuario %s su turno es el numero 41, empieza el dia Jueves a las %d:00 y termina a las %d:15.",nom,hora,hora); val=41; jue++; jueh=jueh+hora;
				      break;
				      case 2: printf("\nUsuario %s su turno es el numero 42, empieza el dia Jueves a las %d:15 y termina a las %d:30.",nom,hora,hora); val=42; jue++; jueh=jueh+hora;
				      break;
				      case 3: printf("\nUsuario %s su turno es el numero 43, empieza el dia Jueves a las %d:30 y termina a las %d:45.",nom,hora,hora); val=43; jue++; jueh=jueh+hora;
				      break;
				      case 4: printf("\nUsuario %s su turno es el numero 44, empieza el dia Jueves a las %d:45",nom,hora); hora=hora+1; printf(" y termina a las %d:00.",hora); val=44; jue++; jueh=jueh+hora-1;
				      break;
				      default: printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario se le invita regresar al menu. Gracias por su comprension.");
				      break;
				      }
				}
				rep=0;} 
				else{ printf("\nLo sentimos, no se encuentran turnos disponibles a esta hora seleccionada. Si desea terminar de agregar, porfavor digite 0, en caso que desee escoger otro horario, digite cualquier otro numero y presione enter: "); scanf("%d",&rep); }
				} while(rep!=0);
					
					break;
				
				case 5: do{ printf("\nSe utilizara un sistema de 24 hrs.\nPor ejemplo, si desea ingresar el horario de las 3 pm, usted debe digitar el numero 15 (que representa a las 3 pm).\n");
				printf("\nDigite por favor el horario donde posee disponibilidad: "); scanf("%d",&hora);
				if(hora>=8 && hora<=19){ printf("\nLas cajas de FIME abren de 8:30 - 19:00. Por lo que es necesario que seleccione un horario disponible.");
				printf("\nIngrese porfavor un numero que representa el lapso del tiempo en donde tiene disponible: ");
				printf("\n1.- 0 a 15 minutos de la hora\n2.- 15 a 30 minutos de la hora\n3.- 30 a 45 minutos de la hora\n4.- 45 a 60 minutos de la hora\nDigite numero: "); scanf("%d",&min);
				if(hora==8 && min>=1 && min<=2){ printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario le invitamos a que regrese al menu para agregar su turno. Gracias por su comprension."); }
				else{ switch(min){ 
				      case 1: printf("\nUsuario %s su turno es el numero 51, empieza el dia Viernes a las %d:00 y termina a las %d:15.",nom,hora,hora); val=51; vie++; vieh=vieh+hora;
				      break;
				      case 2: printf("\nUsuario %s su turno es el numero 52, empieza el dia Viernes a las %d:15 y termina a las %d:30.",nom,hora,hora); val=52; vie++; vieh=vieh+hora;
				      break;
				      case 3: printf("\nUsuario %s su turno es el numero 53, empieza el dia Viernes a las %d:30 y termina a las %d:45.",nom,hora,hora); val=53; vie++; vieh=vieh+hora;
				      break;
				      case 4: printf("\nUsuario %s su turno es el numero 54, empieza el dia Viernes a las %d:45",nom,hora); hora=hora+1; printf(" y termina a las %d:00.",hora); val=54; vie++; vieh=vieh+hora-1;
				      break;
				      default: printf("\nLo sentimos, no hay horarios disponibles en ese horario. Si desea escoger algun otro horario se le invita regresar al menu. Gracias por su comprension.");
				      break;
				      }
				}
				rep=0;} 
				else{ printf("\nLo sentimos, no se encuentran turnos disponibles a esta hora seleccionada. Si desea terminar de agregar, porfavor digite 0, en caso que desee escoger otro horario, digite cualquier otro numero y presione enter: "); scanf("%d",&rep); }
				} while(rep!=0);
					
					break;
									
				default: printf("\nLo sentimos, no poseemos horario para ese dia, puede regresar al menu."); rep=0;
				break;	
			}
				
			
		}while(rep!=0); 
	}
}

void push(int val)
{
    if(top==4)
        printf("\nEl ultimo turno no se agrego correctamente debido a que ya no puede agregar mas turnos.");
    else
    {   if(lun==2 || mar==2 || mie==2 || jue==2 || vie==2){printf("\n\nEl ultimo turno no se agrego correctamente debido a que ya no puede escoger turno para ese dia."); }
        else { top++;
        tr[top] = val;
		}
    }
}

int pop()
{
    
    if(top==-1)
    {
        printf("\nNo hay turnos asignados.\n");
        return -1;
    }
    else
    {
        val = tr[top];
        top--;
        return val;
    }
}

void display()
{
    int i;
    if(top==-1){printf("\nNo hay turnos asignados.\n\n");	}
        
    else
    {
        printf("\nLos turnos asignados son:\n");
        for(i=top; i>=0; i--){printf("\n\n%d:  ", tr[i]);
        switch(tr[i]){
        	case 11: printf("Empieza el dia Lunes a las %d:00 y termina a las %d:15.\n",lunh,lunh); 
        	break;
        	case 12: printf("Empieza el dia Lunes a las %d:15 y termina a las %d:30.\n",lunh,lunh); 
        	break;
        	case 13: printf("Empieza el dia Lunes a las %d:30 y termina a las %d:45.\n",lunh,lunh); 
        	break;
        	case 14: printf("Empieza el dia Lunes a las %d:45",lunh); lunh=lunh+1; printf(" y termina a las %d.\n",lunh); 
        	break;
        	case 21: printf("Empieza el dia Martes a las %d:00 y termina a las %d:15.\n",marh,marh); 
        	break;
        	case 22: printf("Empieza el dia Martes a las %d:15 y termina a las %d:30.\n",marh,marh); 
        	break;
        	case 23: printf("Empieza el dia Martes a las %d:30 y termina a las %d:45.\n",marh,marh); 
        	break;
        	case 24: printf("Empieza el dia Martes a las %d:45",marh); marh=marh+1; printf(" y termina a las %d.\n",marh); 
        	break;
        	case 31: printf("Empieza el dia Miercoles a las %d:00 y termina a las %d:15.\n",mieh,mieh); 
        	break;
        	case 32: printf("Empieza el dia Miercoles a las %d:15 y termina a las %d:30.\n",mieh,mieh); 
        	break;
        	case 33: printf("Empieza el dia Miercoles a las %d:30 y termina a las %d:45.\n",mieh,mieh); 
        	break;
        	case 34: printf("Empieza el dia Miercoles a las %d:45",mieh); mieh=mieh+1; printf(" y termina a las %d.\n",mieh); 
        	break;
        	case 41: printf("Empieza el dia Jueves a las %d:00 y termina a las %d:15.\n",jueh,jueh); 
        	break;
        	case 42: printf("Empieza el dia Jueves a las %d:15 y termina a las %d:30.\n",jueh,jueh); 
        	break;
        	case 43: printf("Empieza el dia Jueves a las %d:30 y termina a las %d:45.\n",jueh,jueh); 
        	break;
        	case 44: printf("Empieza el dia Jueves a las %d:45",jueh); jueh=jueh+1; printf(" y termina a las %d.\n",jueh); 
        	break;
        	case 51: printf("Empieza el dia Viernes a las %d:00 y termina a las %d:15.\n",vieh,vieh); 
        	break;
        	case 52: printf("Empieza el dia Viernes a las %d:15 y termina a las %d:30.\n",vieh,vieh); 
        	break;
        	case 53: printf("Empieza el dia Viernes a las %d:30 y termina a las %d:45.\n",vieh,vieh); 
        	break;
        	case 54: printf("Empieza el dia Viernes a las %d:45",vieh); vieh=vieh+1; printf(" y termina a las %d.\n",vieh); 
        	break;
        
		}
		}
            
    }
}
