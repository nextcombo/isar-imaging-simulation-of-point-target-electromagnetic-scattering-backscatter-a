# ISAR Imaging: Simulation of Point Target Electromagnetic Scattering Backscatter and Research on ISAR Imaging Method [Attached MATLAB Code]

MATLAB simulation results  
MATLAB code
clear all;\nclose all;\nclc;\nC=3e8;               %Light Speed\nima=sqrt(-1);        % Imaginary unit\n%% Scene Center Parameters\nR0=2e4;              % Scene Center Oblique Distance\n%% Radar parameters\nfc=10e9;             % Working frequency 10GHz\nlamda=C/fc;          % Wavelength\nSNR=-10;\n%% Antenna Parameters\nD=4;                 % Antenna aperture length\nLsar=lamda*R0/D;     % Radar Synthetic Aperture Length\n%% Distance to parameter\nTr=10e-6;            % Pulse width at emission\nB=180e6;             % Bandwidth\nKr=B/Tr;             % Frequency adjustment\nFsr=200e6;           % Distance Sampling Rate\nnrn_Tr=Fsr*Tr;       %Pulse interval sampling number\nnrn=2048;            % Distance to sampling number\ntnrn=2*R0/C+[-nrn/2:nrn/2-1]'/Fsr;  % Distance to fast time\n%% azimuth parameters\nFa=100;              % Azimuth Sampling Rate\nPRF=500;             %Pulse repetition frequency\nV=100;               % Aircraft speed\nar=5;                % Aircraft Acceleration\nnan=512;             % Azimuth Sample Number\ntnan=[-nan/2:nan/2-1]/PRF;  % Directional slow time\n%% resolution parameters\nDY=C/2/B;           % Distance to resolution\nDX=DY;              % To maintain the same distance resolution and azimuth resolution, the image scale is consistent.\nwt=lamda/(2*DX*(nan/PRF));   % Angular resolution in the azimuth direction, calculated to determine how much angle wt should be turned. wt is equal to the angular velocity * accumulated time\n%% Target parameters, airplane shape\nNtarget=11;         % Point target count\ndeltaX=15;\ndeltaY=15;\npoints=zeros(Ntarget,3);              \npoints(:,1)=[2*deltaX;deltaX;deltaX;0;0;0;0;0;-deltaX;-deltaX;-2*deltaX];\npoints(:,2)=[0;0;-2*deltaY;2*deltaY;deltaY;0;-deltaY;-2*deltaY;0;-2*deltaY;0];\npoints(:,3)=ones(Ntarget,1);\nfigure(1);\n% h=stem(points(:,1),points(:,2),'fill');\nplot3(points(:,1),points(:,2),points(:,3),'*');\ngrid on;\n% set(h,'LineStyle','none');\naxis([-50 50 -50 50 -5 5])\naxis equal\ntitle('Point target real image');xlabel('x');ylabel('y');\n  

## Images

![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](01.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](02.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](03.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](04.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](05.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](06.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](07.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](08.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](09.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](10.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](11.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](12.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](13.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](14.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](15.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](16.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](17.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](18.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](19.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](20.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](21.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](22.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](23.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](24.jpg)
![(ISAR Imaging)Aircraft Point Target Electromagnetic Scattering Backscatter Simulation and ISAR Imaging Method Research [Attached MATLAB Code]](25.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
