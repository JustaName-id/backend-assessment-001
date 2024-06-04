# backend-assessment-001

### Objective:

Integrate the JustaName SDK (@justaname.id/sdk @justaname.id/react) into a platform, utilizing a React frontend and a NestJS backend. The claiming logic should be handled from the backend and the frontend should call an API to claim the subnames

### Tasks:

1. **Register an ENS Domain on Sepolia Testnet**
    - Set up an Ethereum wallet if you haven’t.
    - Use a Sepolia faucet to get test ETH.
    - Register an ENS domain on the Sepolia testnet.
2. **Access the JustaName Admin Dashboard**
    - Go to [JustaName Admin Dashboard](https://dashboard.justaname.id/).
    - Import your newly registered ENS domain.
    - Generate an API key.
3. **Create a Claim Page with Two Options**
    - Develop a frontend page where users can claim subdomains.
    
    **Features:**
    
    - *Claim Normal Subdomain:* Allow users to claim standard subdomains.
    - *Claim Admin Subdomain:* Enable users to claim admin subdomains at the root domain level. Include a `textRecord` for admin subdomains as follows:
        
        ```json
        {
           "key": "admin",
           "value": "[\"subname1.example.eth\"]"
        }
        ```
        
    
4. **Bonus Task: Create an Admin-Only Page**
    - Implement Sign-In with Ethereum (SIWE) login mechanism.
    - Develop a page that is accessible only to users with admin subdomains.

### Deliverables:

1. Source code (Frontend and Backend) hosted on a Git repository.
2. Documentation outlining how to set up, run, and test your solution.
3. Demonstration video (optional but encouraged) showcasing the functionality of your application.

### Evaluation Criteria:

- Correct integration of the JustaName SDK.
- Functionality of the claim options.
- Implementation of the admin-specific functionalities.
- Code quality and documentation.
- Software Design & Practices (SOLID principles, Testing (unit, integration…), design patterns)
- Bonus points for successfully implementing the admin-only page with SIWE login.
- Bonus points for successfully dockerizing the backend
- Bonus point: Demonstrate possible solutions for scaling the application (if applicable)

Resources:
- https://docs.justaname.id
- https://docs.ethers.org/v6/
- https://metamask.io/
- https://faucet.quicknode.com/ethereum/sepolia
- https://app.ens.domains/
- https://medium.com/@kaishinaw/signing-in-with-ethereum-owning-your-own-identity-a5714f1afcdc
- https://docs.login.xyz/

Contact [ghadi@justalab.co](mailto:ghadi@justalab.co) or hadi@justalab.co for unclear instructions
