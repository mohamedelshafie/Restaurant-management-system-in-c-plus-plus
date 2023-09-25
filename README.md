# Restaurant-management-system-in-c-plus-plus
A complete system for a restaurant using OOP and Data Structures concepts.
## First: The orders:
### Arrival time stamp (in time steps).
### Order type: Normal, Vegan, or VIP.
### Order size (in number of dishes).
### Order price (in L.E.).
## Second: The cooks:
### Specialization: Normal, Vegan, or VIP.
### Break duration: (in time steps).
### Cooking speed: the number of dishes it can prepare in one timestep.
## Third: Order service criteria:
### To determine the next order to serve(priority between different types of orders):
#### For VIP orders, prepared by VIP cooks, if not available then prepared by normal cooks, if not available then prepared by vegan cooks.
#### For normal orders, prepared by normal cooks, if not available then prepared by vegan cooks.
#### For vegan orders, prepared by vegan cooks only.
#### If an order cannot be served at the current time step, it should wait for the next time step to be checked if it can be serviced or not. If not, it should wait again.
### priority between the same types of orders:
#### For vegan & normal orders, First Come First Serve.
#### For VIP orders, by a priority equation that depends on order arrival time, price and size.
### Some additional services for normal orders:
#### Normal orders can be promoted to VIP orders by paying more money.
#### Normal orders can be cancelled as long as it is not assigned to a cook yet.
#### If a Normal order waits more than N timesteps from its arrival time without being assigned to a cook, it will be automatically promoted to be a VIP order.
