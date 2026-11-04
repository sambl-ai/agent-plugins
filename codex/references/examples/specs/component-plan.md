# Selected screen dependency plan

The user selects only a screen. Resolve and build its missing sources internally
in dependency order, self-checking each before reuse; no component selection or
independent review is required from the user. Sources remain generic unless a
specific source WHAT declares a screen preset. Reuse compatible shared sources.

Sign In: Auth Shell, then Sign In screen. No other product families are needed.

Dashboard: Menu Item; Title Block; Account Item; Nav Bar;
Workflow Item; Client Cell; Menu Group (Menu Item); Menu (Menu Group, Account Item);
Navigation (Menu); Dashboard Shell (Navigation, Nav Bar and full navigation closure);
then Dashboard. Only actual retained modes are built. Dashboard
Shell includes its complete navigation preset in every retained source variant,
including hidden compact backings. Call the selected example Dashboard. No additional screen is created.

The per-component WHAT is under components/. The two screen WHAT documents are
sign-in.md and dashboard.md, with their selected kit/content units.
Do not generate Support, Account, Delete confirmation, Popup, Copyable Value or
any other unselected screen/product family.
