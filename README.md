# opencl-device-info
A simple script to check some of the basic information about the OpenCL devices available in your system.

# Linux
```
$ gcc -o deviceInfoQuery deviceInfoQuery.c -lOpenCL
$ ./deviceInfoQuery
```

# MAC
```
$ clang -framework OpenCL deviceInfoQuery.c -o deviceInfoQuery
$ ./deviceInfoQuery
```

Sample output:
```
Starting OpenCL device query: 
------------------------------

 Number of OpenCL capable platforms available: 1 
--------------------------------------------------

	 Platform ID: 0 
	 ----------------

		 [Platform 0] CL_PLATFORM_NAME: Apple
		 [Platform 0] CL_PLATFORM_VENDOR: Apple
		 [Platform 0] CL_PLATFORM_VERSION: OpenCL 1.2 (Oct 31 2017 18:30:00)
		 [Platform 0] CL_PLATFORM_PROFILE: FULL_PROFILE
		 [Platform 0] CL_PLATFORM_EXTENSIONS: cl_APPLE_SetMemObjectDestructor cl_APPLE_ContextLoggingFunctions cl_APPLE_clut cl_APPLE_query_kernel_names cl_APPLE_gl_sharing cl_khr_gl_event

		 [Platform 0] Number of devices available: 2 
		 ---------------------------------------------

			 [Platform 0] Device ID: 0
			 ---------------------------

					 [Platform 0] [Device 0] CL_DEVICE_NAME: Intel(R) Core(TM) i5-6360U CPU @ 2.00GHz
					 [Platform 0] [Device 0] CL_DEVICE_VERSION: OpenCL 1.2 
					 [Platform 0] [Device 0] CL_DRIVER_VERSION: 1.1
					 [Platform 0] [Device 0] CL_DEVICE_OPENCL_C_VERSION: OpenCL C 1.2 
					 [Platform 0] [Device 0] CL_DEVICE_MAX_CLOCK_FREQUENCY: 2000 MHz
					 [Platform 0] [Device 0] CL_DEVICE_MAX_COMPUTE_UNITS: 4
					 [Platform 0] [Device 0] CL_DEVICE_GLOBAL_MEM_SIZE: 8192 MB
					 [Platform 0] [Device 0] CL_DEVICE_MAX_MEM_ALLOC_SIZE: 2048 MB
					 [Platform 0] [Device 0] CL_DEVICE_LOCAL_MEM_SIZE: 32 KB
					 [Platform 0] [Device 0] CL_DEVICE_MAX_WORK_GROUP_SIZE: 1024
					 [Platform 0] [Device 0] CL_DEVICE_MAX_WORK_ITEM_DIMENSIONS: 3
					 [Platform 0] [Device 0] CL_DEVICE_MAX_WORK_ITEM_SIZES: 1024 1 1 
					 [Platform 0] [Device 0] CL_DEVICE_IMAGE_SUPPORT: 1 (Available)
					 [Platform 0] [Device 0] CL_DEVICE_IMAGE2D_MAX_WIDTH: 8192
					 [Platform 0] [Device 0] CL_DEVICE_IMAGE2D_MAX_HEIGHT: 8192
					 [Platform 0] [Device 0] CL_DEVICE_IMAGE3D_MAX_WIDTH: 2048
					 [Platform 0] [Device 0] CL_DEVICE_IMAGE3D_MAX_HEIGHT: 2048
					 [Platform 0] [Device 0] CL_DEVICE_IMAGE3D_MAX_DEPTH: 2048


			 [Platform 0] Device ID: 1
			 ---------------------------

					 [Platform 0] [Device 1] CL_DEVICE_NAME: Intel(R) Iris(TM) Graphics 540
					 [Platform 0] [Device 1] CL_DEVICE_VERSION: OpenCL 1.2 
					 [Platform 0] [Device 1] CL_DRIVER_VERSION: 1.2(Dec 19 2017 21:05:50)
					 [Platform 0] [Device 1] CL_DEVICE_OPENCL_C_VERSION: OpenCL C 1.2 
					 [Platform 0] [Device 1] CL_DEVICE_MAX_CLOCK_FREQUENCY: 1000 MHz
					 [Platform 0] [Device 1] CL_DEVICE_MAX_COMPUTE_UNITS: 48
					 [Platform 0] [Device 1] CL_DEVICE_GLOBAL_MEM_SIZE: 1536 MB
					 [Platform 0] [Device 1] CL_DEVICE_MAX_MEM_ALLOC_SIZE: 384 MB
					 [Platform 0] [Device 1] CL_DEVICE_LOCAL_MEM_SIZE: 64 KB
					 [Platform 0] [Device 1] CL_DEVICE_MAX_WORK_GROUP_SIZE: 256
					 [Platform 0] [Device 1] CL_DEVICE_MAX_WORK_ITEM_DIMENSIONS: 3
					 [Platform 0] [Device 1] CL_DEVICE_MAX_WORK_ITEM_SIZES: 256 256 256 
					 [Platform 0] [Device 1] CL_DEVICE_IMAGE_SUPPORT: 1 (Available)
					 [Platform 0] [Device 1] CL_DEVICE_IMAGE2D_MAX_WIDTH: 16384
					 [Platform 0] [Device 1] CL_DEVICE_IMAGE2D_MAX_HEIGHT: 16384
					 [Platform 0] [Device 1] CL_DEVICE_IMAGE3D_MAX_WIDTH: 2048
					 [Platform 0] [Device 1] CL_DEVICE_IMAGE3D_MAX_HEIGHT: 2048
					 [Platform 0] [Device 1] CL_DEVICE_IMAGE3D_MAX_DEPTH: 2048
```

