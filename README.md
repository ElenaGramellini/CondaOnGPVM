# CondaOnGPVM
On your laptop do:
> port_uboonegpvm 1

where
in your bash_profile you have
port_uboonegpvm(){
         ssh -KXYL localhost:8889:localhost:8889 elenag@uboonebuild0$1.fnal.gov
}


On the gpvm do:
> activateConda

where 
alias activateConda='eval "$(/uboone/app/users/elenag/Miniconda3/bin/conda shell.bash hook)"'

once conda is activated do
> jupiter-lab

close the gpvm browser cause that takes forever.
Copy the http:// link to local browser and enjoy.