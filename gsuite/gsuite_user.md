---
description: gsuite_user
---

# user

Schema
```
{
	addresses: List<Address>,
	agreedToTerms: Boolean,
	aliases: List<String>,
	archived: Boolean,
	changePasswordAtNextLogin: Boolean,
	creationTime: String,
	customerId: String,
	deletionTime: String,
	emails: List<Email>,
	externalIds: List<ExternalId>,
	gender: Gender,
	id: String,
	ims: List<Im>,
	includeInGlobalAddressList: Boolean,
	ipWhitelisted: Boolean,
	isAdmin: Boolean,
	isDelegatedAdmin: Boolean,
	isEnforcedIn2Sv: Boolean,
	isEnrolledIn2Sv: Boolean,
	isMailboxSetup: Boolean,
	keywords: List<Keyword>,
	languages: List<Language>,
	lastLoginTime: String,
	locations: List<Location>,
	name: Name,
	nonEditableAliases: List<String>,
	orgUnitPath: String,
	organizations: List<Organization>,
	phones: List<Phone>,
	posixAccounts: List<PosixAccount>,
	primaryEmail: String,
	recoveryEmail: String,
	recoveryPhone: String,
	relations: List<Relation>,
	sshPublicKeys: List<SshPublicKey>,
	suspended: Boolean,
	suspensionReason: String,
}
```
