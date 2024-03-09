# Automatix

## Description

Automatix is a tool designed to address the challenges of model transformations within the Model-Driven Engineering (MDE) paradigm. Model transformations are crucial for the success of MDE, yet they are fraught with potential syntactic and semantic errors due to the complexity of understanding both the desired transformation and the mechanism of enactment. These errors are not only common but also time-consuming to identify and rectify.

To mitigate these issues, Automatix leverages an evolutionary algorithm (EA) approach to automatically repair ATL transformations containing multiple semantic errors. We introduce the concept of social diversity as an additional objective for our EA. This innovation promotes the generation of repair patches that address a wider range of errors, particularly those less covered by other patches within the population.

Our tool has been evaluated on four mutated ATL transformations, intentionally injected with up to five semantic errors each. The results demonstrate that incorporating social diversity significantly enhances the quality of repair patches and accelerates the repair process, even in the presence of multiple semantic errors.

## Publications
[1] VaraminyBahnemiry, Z., Galasso, J., Belharbi, K., & Sahraoui, H. (2021, October). Automated Patch Generation for Fixing Semantic Errors in ATL Transformation Rules. In 2021 ACM/IEEE 24th International Conference on Model Driven Engineering Languages and Systems (MODELS) (pp. 13-23). IEEE.

## Getting Started

Automatix is built to work within the Eclipse ecosystem, leveraging a suite of MDE tools and dependencies to provide its advanced model transformation repair capabilities. To ensure smooth operation, the following prerequisites must be met:

### Environment
- **Java Development Kit (JDK):** JavaSE-14 or higher is required for running Automatix.

### Eclipse Plugins and Dependencies
Automatix integrates with several Eclipse plugins and external dependencies. Ensure that your Eclipse environment includes the following bundles:

- **Eclipse Core Runtime**
- **Apache Log4j:** `bundle-version="1.2.15"`
- **AnATLyzer ATL Typing:** `bundle-version="0.1.0"`
- **Eclipse M2M ATL Core and EMF:** Various versions, including `bundle-version="4.2.2"` for core ATL functionalities.
- **AnATLyzer ATL Tests API:** `bundle-version="0.1.0"`
- **AnATLyzer Use Witness:** `bundle-version="0.1.0"`
- **Eclipse EMF (Eclipse Modeling Framework):** `bundle-version="2.8.0"`, and other related EMF packages.
- **Eclipse M2M ATL DSLs, Common, Engine, EMFTVM:** Ensuring support for ATL model transformations and execution.
- **Eclipse UI Workbench and JFace:** For UI support within Eclipse.
- **Eclipse Core Resources:** `bundle-version="3.13.800"`
- **ObjectWeb ASM:** `bundle-version="8.0.1"` for bytecode manipulation.
- **Eclipse EMF Transaction and EMF Compare:** Including diagram support with `bundle-version="2.5.2"`
- **Google Guava:** `bundle-version="21.0.0"` for core libraries.
- **Eclipse M2M ATL ADT Editor:** For ATL development tools.
- **Eclipse JFace Data Binding:** For UI data binding support.

### Installation

To integrate Automatix with your Eclipse setup, follow these steps:

1. Ensure your Eclipse environment meets the JDK and plugin dependencies listed above.
2. Import the Automatix projects within your Eclipse installation.
3. Set up the transformation files, following the folder structure.

### Usage

1. Run the main method in the class `cd.udem.fixingatlerror/src/cd/udem/fixingatlerror/Class2Ref.java'.

## Contact Information

For more information on Automatix, please contact `sahraouh@iro.umontreal.ca`.
