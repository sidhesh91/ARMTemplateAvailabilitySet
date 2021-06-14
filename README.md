# Repository for custom azure ARM templates 

genral purpose:
B, Dsv3, Dv3, Dasv4, Dav4, DSv2, Dv2, Av2, DC, DCv2, Dv4, Dsv4, Ddv4, Ddsv4

optimezed
F, Fs, Fsv2

memory optimezed:
Esv3, Ev3, Easv4, Eav4, Ev4, Esv4, Edv4, Edsv4, Mv2, M, DSv2, Dv2



Disk type	SSD	SSD	SSD	HDD
Disk capacity: Ultra disks capacity ranges from 4 GiB up to 64 TiB.


Premium SSD sizes 	P1	P2	P3	P4	P6	P10	P15	P20	P30	P40	P50	P60	P70	P80
Disk size in GiB	4	8	16	32	64	128	256	512	1,024	2,048	4,096	8,192	16,384	32,767



az storage account create \
    --name <storage-account> \
    --resource-group <resource-group> \
    --location <location> \
    --sku Standard_ZRS \
    --encryption-services blob
  
  
  
  az storage container create \
    --account-name <storage-account> \
    --name <container> \
    --auth-mode login
  
  az storage blob upload \
    --account-name <storage-account> \
    --container-name <container> \
    --name helloworld \
    --file helloworld \
    --auth-mode login
  
  
  az keyvault create --resource-group --name
  --enabled-for-deployment
  
  
  az group create --name myResourceGroup --location westus
  
  az webapp up --name <your_app_name> --logs --launch-browser
  
  az appservice plan create -g MyResourceGroup -n MyPlan
  
  az appservice plan create -g MyResourceGroup -n MyPlan \
    --is-linux --number-of-workers 4 --sku S1
  
  
  
  
  
