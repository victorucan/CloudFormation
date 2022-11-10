empty:
	@echo ""


delete-staging:
	aws cloudformation delete-stack --stack-name staging-conditionals 
deploy-staging:
	aws cloudformation deploy --stack-name staging-conditionals --template-file stack-conditionals.yml --parameter-overrides KeyParameter=jenk-nw VpcIdParameter=vpc-0fb2c2fa3c3cae44b AmiIdParameter=ami-08c40ec9ead489470 Environment=staging



delete-prod:
	aws cloudformation delete-stack --stack-name prod-conditionals 
deploy-prod:
	aws cloudformation deploy --stack-name prod-conditionals --template-file stack-conditionals.yml --parameter-overrides KeyParameter=jenk-nw VpcIdParameter=vpc-0fb2c2fa3c3cae44b AmiIdParameter=ami-08c40ec9ead489470 Environment=prod