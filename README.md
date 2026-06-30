# Simplified BCPNN implementation
 
My BCPNN implementation

A Bayesian confidence propagation neural network is a Bayesian neural network that is based on a Hebbian learning rule (known popularly by the aphorism "Cells that wire together, fire together"). It describes a synaptic learning rule for neuromorphic computing, and was developed by Dr. Anders Lansner and Dr. Örjan Ekeberg at the Royal Institute of Technology in Stockholm, Sweden. 

The implementation of the BCPNN here is to do with the synaptic trace-based learning rule, and how to implement the synaptic traces, represented by a sequence of first order ordinary differential equations. The paper goes into the analog circuit-level implementation of the BCPNN, which involves simulating for the solutions of these differential equations. A simplified BCPNN learning rule involves the omission of the E-trace, which is what this implementation entails. 

On a very basic level what is being done is implementing the simplified BCPNN by utilizing the solutions to the differential equations describing the traces.  

The main struggle I encountered early on was being unable to generate the spiking inputs. The initial attempt (found in the master branch) includes code that is 80% correct, but where the spikes were implemented by trying to convert an image into a spiking input, an incorrect and needlessly complicated approach. This is why you see traces that look nothing like what's described in the paper. It was only when I introduced the idea of spiking probability that you begin to see spiking inputs that match what is described in the paper. 

If you have questions about the implementation, please reach out to me. 
