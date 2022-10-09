# Class-Reccomennder
Allows users to key in classes they have taken which the system then recommend a class from the list of classes they are eligible for.

Using McgGill database for classes from the faculty of Science, we cleaned the data into columns of pre-requisites before fine-tuning a Genism Word2Vec model using the description of the classes and we evaluate classes similarity based on the cosine similarity between the word-embeddings of the class description.

Google Colab code: https://colab.research.google.com/drive/1qEcACGjaMIVokQiKXQnzX7s9nSfJtByP#scrollTo=CPRHyfgK8gcV

## E.g
running: reccomend("MATH 133", ["COMP 251", 'COMP 206' , 'COMP 250', 'COMP 251', 'MATH 323', 'COMP 324', 'MATH 240', "MATH 222", "MATH 133"],df)
returns the following:

Course input : MATH 133
Course Name Linear Algebra and Geometry.
Description: Systems of linear equations, matrices, inverses, determinants; geometric vectors in three dimensions, dot product, cross product, lines and planes; introduction to vector spaces, linear dependence and independence, bases. Linear transformations. Eigenvalues and diagonalization.


Class #1 : MATH 223  
Course Name: Linear Algebra. 
Description: Review of matrix algebra, determinants and systems of linear equations. Vector spaces, linear operators and their matrix representations, orthogonality. Eigenvalues and eigenvectors, diagonalization of Hermitian matrices. Applications. 
Average Professor rating: NIL 

Class #2 : MATH 248  
Course Name: Honours Vector Calculus. 
Description: Partial derivatives and differentiation of functions in several variables; Jacobians; maxima and minima; implicit functions. Scalar and vector fields; orthogonal curvilinear coordinates. Multiple integrals; arc length, volume and surface area. Line and surface integrals; irrotational and solenoidal fields; Green's theorem; the divergence theorem. Stokes' theorem; and applications. 
Average Professor rating: 4.5 

Class #3 : MATH 314  
Course Name: Advanced Calculus. 
Description: Derivative as a matrix. Chain rule. Implicit functions. Constrained maxima and minima. Jacobians. Multiple integration. Line and surface integrals. Theorems of Green, Stokes and Gauss. Fourier series with applications. 
Average Professor rating: NIL 

Class #4 : MATH 315  
Course Name: Ordinary Differential Equations. 
Description: First order ordinary differential equations including elementary numerical methods. Linear differential equations. Laplace transforms. Series solutions. 
Average Professor rating: NIL 

Class #5 : MATH 140  
Course Name: Calculus 1. 
Description: Review of functions, exponents and radicals, exponential and logorithm. Examples of functions in business applications. Limits, continuity and derivatives. Differentiation of elementary functions. Antiderivatives. The definite integral. Techniques of Integration. Applications of differentiation and integration including differential equations. Trigonometric functions are not discussed in this course. 
Average Professor rating: 4.5 

