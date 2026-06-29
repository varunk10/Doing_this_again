# Simplified BCPNN implementation
 
My BCPNN implementation

On a very basic level what is being done is implementing the BCPNN (simplified, without including the E-traces) by utilizing the solutions to the differential equations describing the traces. 


The main struggle I encountered early on was being unable to generate the spiking inputs. The initial attempt includes code that is 80% correct, but where the spiking inputs were implemented by trying to convert an image into a spiking input, an incorrect and needlessly complicated approach. This is why you see traces that look nothing like what's described in the paper. 

If you have questions about the implementation, please reach out to me. 
